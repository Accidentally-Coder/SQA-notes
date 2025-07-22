---


---

<h1 id="lecture-1--overview-and-basic-definitions">Lecture 1 : Overview and Basic Definitions</h1>
<h4 id="what-is-a-computer-program">What is a computer program?</h4>
<ul>
<li>Regular defn : set of instructions for a computer</li>
<li>In reality,
<ul>
<li>not just code/instructions - it’s a communication tool among stakeholders who are distributed over space and time</li>
<li>built to deliver value to the people(stakeholders), not just functionality to a machine</li>
</ul>
</li>
</ul>
<h4 id="who-are-stakeholders">Who are stakeholders?</h4>
<p>Any person affected by:</p>
<ul>
<li>success/failure</li>
<li>actions/inactions</li>
<li>effects<br>
of a project/product/service</li>
</ul>
<h4 id="what-is-bug">What is bug?</h4>
<ul>
<li>An attribute of a software product that reduces its value to the favored stakeholders.</li>
</ul>
<h4 id="what-is-software-testing">What is software testing?</h4>
<ul>
<li>An <strong>empirical</strong>, <strong>technical</strong> <strong>investigation</strong> conducted to provide <strong>stakeholders</strong> with <strong>information</strong> about the <strong>quality</strong> of the product or service under test.</li>
<li>Goal: <strong>Gain useful information</strong>, not just find bugs</li>
<li>Involves <strong>investigation</strong>, <strong>interpretation</strong>, and <strong>judgement</strong></li>
</ul>
<h5 id="detailed-breakdown-of-the-definition">Detailed Breakdown of the Definition</h5>

<table>
<thead>
<tr>
<th>Term</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td>Empirical</td>
<td>Based on observation, experimentation, not just theory</td>
</tr>
<tr>
<td>Technical</td>
<td>Uses logical reasoning, models, tools, data</td>
</tr>
<tr>
<td>Investigation</td>
<td>Organized inquiry to find important information</td>
</tr>
<tr>
<td>Stakeholders</td>
<td>Anyone invested in the product’s success or failure</td>
</tr>
<tr>
<td>Information</td>
<td>Typically about bugs, but also usability, compatibility, risks</td>
</tr>
<tr>
<td>Quality</td>
<td>“Value to some person” (subjective, varies by context) – Weinberg</td>
</tr>
</tbody>
</table><h4 id="why-we-test">Why we test?</h4>
<p>Testing serves various information objectives:</p>
<ul>
<li>Find important bugs</li>
<li>Assess product quality and readiness</li>
<li>Help with release decisions</li>
<li>Predict support costs</li>
<li>Check interoperability, conformance, and usability</li>
<li>Minimize risk of legal issues</li>
</ul>
<h3 id="black-box-vs-glass-white-box-testing">Black Box vs Glass (White) Box Testing</h3>

<table>
<thead>
<tr>
<th>Aspect</th>
<th>Black Box</th>
<th>Glass Box (White Box)</th>
</tr>
</thead>
<tbody>
<tr>
<td>Focus</td>
<td>Externally visible behavior</td>
<td>Internals of the code</td>
</tr>
<tr>
<td>Expertise</td>
<td>User needs, market, risks</td>
<td>Code structure and logic</td>
</tr>
<tr>
<td>Code knowledge</td>
<td>Not required</td>
<td>Required</td>
</tr>
<tr>
<td>Design perspective</td>
<td>Tests from user’s view</td>
<td>Tests from developer’s view</td>
</tr>
</tbody>
</table><ul>
<li><strong>Grey Box Testing</strong> – A mix; uses partial knowledge of internals (e.g., log analysis).</li>
</ul>
<h4 id="testing-terminology">Testing terminology</h4>
<ul>
<li>
<p><strong>Behavioral Testing</strong>: Observes program behavior from the outside (usually black box).</p>
</li>
<li>
<p><strong>Structural Testing</strong>: Focuses on code internals (equivalent to glass box).</p>
</li>
<li>
<p><strong>Functional Testing</strong>: Based on system’s expected functions.</p>
</li>
<li>
<p><strong>Parafunctional/Non-functional Testing</strong>: Tests for non-functional aspects (usability, performance, etc.).</p>
</li>
</ul>
<h3 id="test-levels">Test levels</h3>

<table>
<thead>
<tr>
<th>Level</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Unit Testing</td>
<td>Tests individual components/modules</td>
</tr>
<tr>
<td>Integration Testing</td>
<td>Tests interactions between integrated units</td>
</tr>
<tr>
<td>System Testing</td>
<td>Tests complete system against requirements</td>
</tr>
<tr>
<td>Acceptance Testing</td>
<td>Validates whether the software meets contract terms</td>
</tr>
</tbody>
</table><h4 id="independent-testing">Independent Testing</h4>
<ul>
<li>Done by testers not influenced by developers</li>
<li>Can be internal or external</li>
<li>Purpose : Ensure objectivity in test design and evaluation</li>
</ul>
<h1 id="lecture-2--strategy">Lecture 2 : Strategy</h1>
<ul>
<li>Different missions -&gt; Different strategies, tools, and results</li>
</ul>
<h4 id="testing-mission">Testing mission</h4>
<ul>
<li>A mission is focused on <strong>information objectives</strong>.</li>
<li>Avoid mixing too many missions; it leads to a lack of focus.</li>
<li>Mission can <strong>change during the project</strong> (e.g., bug-hunting early, status-checking later).</li>
</ul>
<h4 id="testing-strategy-vs-plan">Testing Strategy vs Plan</h4>

<table>
<thead>
<tr>
<th>Term</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td>Strategy</td>
<td>Ideas guiding <strong>test design</strong></td>
</tr>
<tr>
<td>Logistics</td>
<td>How to apply resources (people, time, tools)</td>
</tr>
<tr>
<td>Plan</td>
<td>Combines strategy, logistics, and risk management</td>
</tr>
</tbody>
</table><h4 id="design-questions-to-shape-test-strategy">Design questions to shape Test Strategy</h4>
<ul>
<li>Who will run the tests?</li>
<li>What skills or tools are needed?</li>
<li>What will be tested vs ignored?</li>
<li>What are oracles ( how will we recognize failure) ?</li>
<li>How will we know when we’re done?</li>
</ul>
<p>**Oracle  : ** A heuristic mechanism by which a tester recognizes a potential problem in the software.</p>
<ul>
<li>Mechanism to determine whether a program passed or failed a test</li>
</ul>
<h3 id="test-techniques">Test techniques</h3>

<table>
<thead>
<tr>
<th>Technique</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Scenario Testing</td>
<td>Real-life use cases; highly credible; stakeholder-relevant</td>
</tr>
<tr>
<td>Domain Testing</td>
<td>Systematic input sampling using partitions, boundaries, and combinations; more likely to trigger failure ;powerful but less credible due to reliance on extreme values</td>
</tr>
</tbody>
</table><ul>
<li><strong>Note:</strong> One test technique ≠ complete testing. You often need several.</li>
</ul>
<h4 id="components-of-a-test-technique-recipe---style">Components of a test technique (Recipe - style)</h4>
<p>(from Domain Testing example):</p>
<ul>
<li>Analyze the situation</li>
<li>Model the test space</li>
<li>Select what to cover</li>
<li>Choose oracles</li>
<li>Configure and operate the test system</li>
<li>Observe and evaluate the results</li>
</ul>
<h1 id="lecture-3--oracles">Lecture 3 : Oracles</h1>
<p>Traditionally,<br>
Oracle : A mechanism for determining whether the program passed or failed a test.</p>
<p>In BBST :<br>
Oracle : A heuristic principle or mechanism that helps testers to recognize a potential problem.</p>
<h4 id="terminology">Terminology</h4>
<ul>
<li>SUT : Software Under Test</li>
<li>AUT : Application Under Test</li>
<li>PUT : Program Under Test</li>
<li>Reference Program / Oracle : If we compare the behavior of SUT with respect to another program, the 2nd program is the reference program or the reference oracle.</li>
<li>Comparator : the software or human that compares the behavior of SUT to the oracle.</li>
</ul>
<h3 id="fallibility-of-oracles">Fallibility of Oracles</h3>

<table>
<thead>
<tr>
<th>Type of Error</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td>False alarm</td>
<td>A correct behavior misjudged as a bug</td>
</tr>
<tr>
<td>Miss</td>
<td>A real bug is overlooked or not recognized</td>
</tr>
</tbody>
</table><h3 id="consistency-oracles">Consistency oracles</h3>
<ul>
<li>Consistent within product : Function behavior consistent with comparable functions within the product</li>
<li>Consistent within comparable products : Function behavior consistent with similar functions in comparable products</li>
<li>Consistent with history : Present behavior consistent with past behaviors</li>
<li>Consistent with our image : Behavior consistent with an image that the organization wants to project</li>
<li>Consistent with claims : Behavior consistent with documentation, specifications or ads</li>
<li>Consistent with standards or regulations : Behavior consistent with externally-imposed requirements</li>
<li>Consistent with user’s expectations : Behavior consistent with what we think users want</li>
<li>Consistent with purpose : Behavior consistent with product’s apparent purpose</li>
</ul>
<h3 id="types-of-oracle-use-cases--doug-hoffmans-model-">Types of Oracle Use Cases ( Doug Hoffman’s Model )</h3>

<table>
<thead>
<tr>
<th>Oracle Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>No oracle (incompetent human)</strong></td>
<td>Just clicking randomly; no evaluation happening</td>
</tr>
<tr>
<td><strong>No oracle (competent human)</strong></td>
<td>Tester uses background knowledge and judgment during testing</td>
</tr>
<tr>
<td><strong>Complete oracle</strong></td>
<td>Very rare; perfect source of truth for comparison</td>
</tr>
<tr>
<td><strong>Heuristic oracle</strong></td>
<td>Common; based on experience, context, patterns</td>
</tr>
<tr>
<td><strong>Heuristic + automated oracle</strong></td>
<td>Tools help judge correctness, but guided by human-developed heuristics</td>
</tr>
</tbody>
</table><h4 id="research-and-credibility">Research and credibility</h4>
<p>To use oracles effectively:</p>
<ul>
<li>Understand the product’s purpose</li>
<li>Research user goals, documentation, competing tools, and support records</li>
<li>Be prepared to defend your judgement with logic and references</li>
</ul>
<h3 id="how-oracles-help-in-testing">How Oracles Help in Testing</h3>

<table>
<thead>
<tr>
<th>Use case</th>
<th>How Oracles Help</th>
</tr>
</thead>
<tbody>
<tr>
<td>Bug evaluation</td>
<td>Justify why behavior is a bug</td>
</tr>
<tr>
<td>Bug reporting</td>
<td>Explain clearly why the issue is important</td>
</tr>
<tr>
<td>Test design</td>
<td>Predict what should/shouldn’t happen based on consistency or claims</td>
</tr>
</tbody>
</table><ul>
<li>Automation doesn’t eliminate the need for oracles</li>
<li>Effective testing = applying the right oracles in the right context</li>
</ul>
<h3 id="guide-in-creating-a-model-modeling-for-test-design">Guide in creating a model (Modeling for Test Design)</h3>
<p>When designing models to guide testing, consider the following aspects of the system:</p>

<table>
<thead>
<tr>
<th>Guide Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Capabilities</strong></td>
<td>What the product can do (features, limits)</td>
</tr>
<tr>
<td><strong>Preferences</strong></td>
<td>What users or stakeholders want (based on competitive analysis, support)</td>
</tr>
<tr>
<td><strong>Chronology</strong></td>
<td>Events in time — task flows or life history of a function or user action</td>
</tr>
<tr>
<td><strong>Sequences of Actions</strong></td>
<td>Step-by-step behavior (e.g., state diagrams, flowcharts)</td>
</tr>
<tr>
<td><strong>Flow of Information</strong></td>
<td>Data movement within the system (e.g., data flow diagrams, protocols)</td>
</tr>
<tr>
<td><strong>Interactions/Dependencies</strong></td>
<td>Logical or functional relationships (e.g., decision trees, dependency graphs)</td>
</tr>
<tr>
<td><strong>Collections</strong></td>
<td>Groupings like categories, taxonomies, or structured lists</td>
</tr>
<tr>
<td><strong>Motives</strong></td>
<td>Stakeholder interests or impacts (who cares, about what, and why)</td>
</tr>
</tbody>
</table><h4 id="more-types-of-oracles">More types of oracles</h4>
<ul>
<li>State model</li>
<li>Interaction model</li>
<li>Calculation oracle</li>
<li>Inverse oracle</li>
<li>Business model</li>
<li>Theoretical model</li>
<li>Reference program</li>
<li>Statistical</li>
<li>Data set with known characteristics</li>
<li>Hand crafted : result crafted by test designer</li>
<li>Human : human decides program acceptability</li>
</ul>

