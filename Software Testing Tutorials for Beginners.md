---


---

<h2 id="software-testing">Software Testing</h2>
<ul>
<li>
<p>Process to identify <strong>correctness</strong>, <strong>completeness</strong> and <strong>quality</strong> of developed software.</p>
</li>
<li>
<p>Process to <strong>find errors</strong> so that it can be corrected before release.</p>
</li>
</ul>
<h2 id="testing-principles">7 testing principles</h2>
<ol>
<li>
<p>Testing shows presence of defects<br>
-Testing can show <strong>bug exists</strong>, but it <strong>can’t</strong> prove they are <strong>all gone</strong>.</p>
</li>
<li>
<p>Exhaustive testing is impossible</p>
</li>
</ol>
<ul>
<li>You can’t test everything, focus on <strong>risk-based</strong> and <strong>prioritized</strong> testing.</li>
</ul>
<ol start="3">
<li>Early testing</li>
</ol>
<ul>
<li>Start testing early in the software lifecycle to catch defects <strong>sooner</strong></li>
<li>Early testing saves <strong>time</strong> and <strong>money</strong></li>
</ul>
<ol start="4">
<li>Defect clustering</li>
</ol>
<ul>
<li><strong>Most bugs</strong> are usually found in a <strong>few modules</strong> (<em><strong>Pareto Principle : 80/20 rule</strong></em>)</li>
</ul>
<ol start="5">
<li>Pesticide paradox</li>
</ol>
<ul>
<li><strong>Repeating</strong> same tests <strong>won’t find bugs</strong>; <strong>update</strong> tests regularly</li>
</ul>
<ol start="6">
<li>Testing is context dependent</li>
</ol>
<ul>
<li>Testing approach <strong>varies</strong> based on <strong>software type</strong></li>
</ul>
<ol start="7">
<li>Absence-of-errors fallacy</li>
</ol>
<ul>
<li>A <strong>bug-free</strong> system is <strong>useless</strong> if it <strong>doesn’t</strong> meet <strong>user needs</strong>.</li>
</ul>
<h4 id="summary">Summary</h4>
<p><strong>DEEP TAP</strong></p>

<table>
<thead>
<tr>
<th>Letter</th>
<th>Principle</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>D</strong></td>
<td><strong>Defect clustering</strong></td>
<td>Most bugs are found in few modules</td>
</tr>
<tr>
<td><strong>E</strong></td>
<td><strong>Exhaustive testing is impossible</strong></td>
<td>You can’t test everything</td>
</tr>
<tr>
<td><strong>E</strong></td>
<td><strong>Early testing</strong></td>
<td>Start testing early to catch bugs sooner</td>
</tr>
<tr>
<td><strong>P</strong></td>
<td><strong>Pesticide paradox</strong></td>
<td>Repeating the same tests won’t reveal new bugs</td>
</tr>
<tr>
<td><strong>T</strong></td>
<td><strong>Testing shows presence of defects</strong></td>
<td>Testing shows bugs exist, not that they’re gone</td>
</tr>
<tr>
<td><strong>A</strong></td>
<td><strong>Absence-of-errors fallacy</strong></td>
<td>A bug-free system isn’t useful if it fails business needs</td>
</tr>
<tr>
<td><strong>P</strong></td>
<td><strong>Testing is context dependent</strong></td>
<td>Testing varies based on project context</td>
</tr>
</tbody>
</table><h2 id="software-testing--sdlc-vs-stlc">Software Testing : SDLC vs STLC</h2>
<h3 id="waterfall-model">Waterfall Model</h3>
<ul>
<li><strong>Linear</strong> and <strong>sequential</strong> software development approach where <strong>each phase</strong> must be <strong>completed</strong>  <strong>before</strong> moving to the <strong>next</strong> phase. \</li>
</ul>
<p>Requirement gather &gt; Design &gt; Build &gt; Test &gt; Maintenance</p>
<ul>
<li>Drawback : Difficult to go back and make changes once a phase is completed</li>
</ul>
<h3 id="v-model-of-testing">V-Model of Testing</h3>
<ul>
<li>An extension of waterfall model where <strong>testing is planned parallelly</strong> with development</li>
</ul>
<p><em>Left side - Development phases (SDLC)<br>
Right side - Testing phases (STLC)</em></p>
<p><strong>Requirement Analysis</strong> - User <strong>Acceptance</strong> Testing<br></p>
<p><strong>System</strong> design / Functional specifications - <strong>System</strong> Testing<br></p>
<p><strong>Architectural</strong> design/ High level design - <strong>Integration</strong> Testing<br></p>
<p><strong>Module</strong> Design / Detailed Design / Program specification - <strong>Unit</strong> testing</p>
<p><strong>Pros</strong></p>
<ul>
<li>
<p>Early testing</p>
</li>
<li>
<p>Clear relationship between development and testing</p>
</li>
</ul>
<p><img src="SQA-notes/images/V-Model.png" alt="V-Model"></p>
<h2 id="iterative-life-cycle">Iterative Life Cycle</h2>
<ul>
<li>Develops software through repeated cycles(iterations).</li>
<li>Each iteration : more functionality and improves the system based on feedback.</li>
</ul>
<p>![Iterative-Life-Cycle](\SQA notes\images\Iterative Life Cycle.png)</p>
<h2 id="unit-testing">Unit Testing</h2>
<ul>
<li>also called <strong>component testing</strong></li>
<li><strong>What is tests :</strong> performed on <strong>standalone module</strong></li>
<li><strong>Purpose:</strong> to check whether it is developed correctly or not</li>
<li>done by <strong>developers</strong></li>
</ul>
<h2 id="integration-testing">Integration Testing</h2>
<ul>
<li><strong>What is tests :</strong> Interaction between <strong>multiple modules</strong></li>
<li><strong>Purpose :</strong> Check that combined modules work together properly</li>
<li>done by <strong>developers or testers</strong></li>
</ul>
<p>To <strong>increase effectiveness</strong> of Integration testing, <strong>top-down</strong> approach can be followed where high level modules will be tested first. In that case, <strong>stub</strong> can be used.</p>
<h4 id="what-is-stub">What is stub?</h4>
<p>A stub is a <strong>temporary piece of code</strong> used to <strong>simulate</strong> the <strong>behavior of lower-level modules</strong> that are not yet developed or available.</p>
<p>OR</p>
<p><strong>bottom-up</strong> approach which requires <strong>drivers</strong>.</p>
<h4 id="what-is-drivers">What is drivers?</h4>
<p>A driver is a <strong>temporary</strong> module or code used to <strong>simulate</strong> a <strong>calling</strong> module**(higher-level component)** that hasn’t been developed yet.</p>
<h2 id="system-testing">System Testing</h2>
<ul>
<li><strong>What is tests :</strong> entire system</li>
<li><strong>Purpose :</strong> <strong>validates</strong> that the complete software meets the <strong>specified requirements</strong></li>
<li>done by <strong>QA or testers</strong></li>
</ul>
<h2 id="user-acceptance-testinguat">User Acceptance Testing(UAT)</h2>
<ul>
<li><strong>What is tests :</strong> whether the system meets <strong>business needs</strong> and is ready for <strong>deployment</strong></li>
<li><strong>Purpose :</strong> Ensure the software is useable, solves the problem, and is acceptable for release</li>
<li>done by <strong>End-users or clients</strong></li>
</ul>
<p>Acceptance testing is of 2 types:</p>
<ol>
<li>Alpha testing</li>
</ol>
<ul>
<li>internal testing</li>
<li><strong>in-house</strong> testing (controlled environment)</li>
<li>a small set of employees of the client; internal testers or QA team</li>
</ul>
<ol start="2">
<li>Beta testing</li>
</ol>
<ul>
<li>external testing</li>
<li>Performed in the <strong>real world</strong>; after alpha testing, before the final release</li>
<li>a small group of customers or external users</li>
</ul>
<h2 id="sanity--smoke-testing">Sanity / Smoke testing</h2>
<ul>
<li>To check <strong>critical functionalities</strong> of the system before it is accepted for major testing</li>
<li>quick and non-exhaustive</li>
<li><strong>goal :</strong> <strong>check system health</strong>; not finding defects</li>
</ul>
<h2 id="maintenance-testing">Maintenance testing</h2>
<ul>
<li><strong>What it is:</strong> Testing done <strong>after the software is release</strong>d and in use</li>
<li><strong>Purpose:</strong> To verify system still works correctly after updates, bug fixes, or enhancements</li>
</ul>
<h3 id="regression-testing">Regression testing</h3>
<ul>
<li><strong>What it is:</strong> Re-testing existing functionality to ensure that <strong>new changes haven’t introduced bugs</strong></li>
<li><strong>Purpose:</strong> To confirm that code modifications don’t break existing features</li>
<li><strong>Often automated</strong> since require repetition</li>
</ul>
<h2 id="non-functional-testing">Non-functional testing</h2>
<ul>
<li>performance, load, usability</li>
</ul>
<h3 id="performance-testing">Performance testing</h3>
<ul>
<li>Check and fine tune system <strong>response time</strong></li>
<li>goal : reduce response time</li>
</ul>
<h3 id="load-testing">Load testing</h3>
<ul>
<li>Check system performance at different load (number of people accessing the system)</li>
</ul>
<h2 id="summary-of-testing-types">Summary of Testing Types</h2>
<p>3 types :</p>
<ol>
<li>Functional testing</li>
</ol>
<ul>
<li>Unit testing</li>
<li>Integration testing</li>
<li>Smoke/Sanity</li>
<li>UAT</li>
<li>Globalization</li>
<li>Interpretability etc</li>
</ul>
<ol start="2">
<li>Non-functional testing</li>
</ol>
<ul>
<li>Performance</li>
<li>Endurance</li>
<li>Load</li>
<li>Volume</li>
<li>Scalability</li>
<li>Usability etc</li>
</ul>
<ol start="3">
<li>Maintenance testing</li>
</ol>
<ul>
<li>Regression</li>
<li>Maintenance</li>
</ul>
<h2 id="test-formality">Test Formality</h2>
<h3 id="test-scenario">Test scenario</h3>
<ul>
<li>A test scenario is any <strong>functionality</strong> of the application <strong>under test</strong></li>
<li>also called test condition or test possibility</li>
</ul>
<h3 id="test-basis">Test Basis</h3>
<ul>
<li>To create test cases, you need to look at something to base your test</li>
<li>Test basis is <strong>what you test against</strong></li>
<li>Test basis refers to the documents, requirements, or information used as the foundation for designing test cases and test scenarios in software testing.</li>
</ul>
<h2 id="test-steps">Test steps</h2>
<p>Fields in a testing documentation:</p>
<ul>
<li>Test scenario</li>
<li>Test case</li>
<li>Pre-conditions</li>
<li>Test step</li>
<li>Test data</li>
<li>Expected result</li>
<li>Actual results</li>
<li>Pass/Fail</li>
</ul>
<h2 id="how-to-create-requirement-traceability-matrixrtm">How to create Requirement Traceability Matrix(RTM)</h2>
<p>RTM(Requirement Traceability Matrix) is a document that <strong>maps requirements to test cases</strong> to ensure every requirement is covered by testing.</p>
<h3 id="structure-of-an-rtm">Structure of an RTM</h3>
<ul>
<li>Req ID</li>
<li>Requirement Description</li>
<li>Test case ID</li>
<li>Test status</li>
<li>Comments</li>
</ul>
<h3 id="how-to-create-rtm">How to create RTM</h3>
<ol>
<li>Collect requirements</li>
<li>Assign Requirement IDs</li>
<li>List test cases</li>
<li>Map test cases to requirements</li>
<li>Update execution status (pass/fail/in progress etc)</li>
<li>Add comments</li>
</ol>
<h3 id="types-of-traceability">Types of traceability</h3>
<ol>
<li>Forward traceability : req -&gt; test cases</li>
<li>Backward traceability : test cases -&gt; req</li>
<li>Bidirectional traceability : tracks both forward and backward</li>
</ol>
<h2 id="testing-techniques">Testing techniques</h2>
<p>Testing techniques are methods used to <strong>design test cases</strong> that effectively validate software functionality and uncover defects.</p>
<h3 id="types-of-testing-techniques">Types of testing techniques</h3>
<p><strong>1. Black Box Testing Techniques</strong><br>
Focus on inputs and outputs <strong>without</strong> knowing internal code.</p>
<ul>
<li>Equivalence Partitioning: Divide input data into <strong>valid/invalid partitions</strong>; test one from each</li>
<li>Boundary value analysis: Test values at the <strong>edges(min/max)</strong> of input ranges. It is also called <em>range checking</em>.</li>
<li>Decision Table Testing: Use tables to model logic based on <strong>combinations of inputs that produce different results.</strong> Possible combinations = 2^n, n = number of input conditions</li>
<li>State transition testing: Test system behavior based on <strong>state changes</strong>.<br>
Diagram called : state chart or graph. There are 4 main components of the graph: <em>states</em>, <em>transition</em>,<em>events</em>(that cause transition)</li>
<li>Use case testing: Design tests from <strong>user interaction</strong> scenarios. This technique helps identify test cases that cover the entire system, on a transaction by transaction basis, from start to finish. Widely used in acceptance test.</li>
</ul>
<p><strong>2. White Box Testing Techniques</strong><br>
Require knowledge of internal code logic.</p>
<ul>
<li>Statement coverage: ensures every line of code is executed at least once</li>
<li>Branch/decision coverage: ensures all branches(e.g., if/else) are tested</li>
<li>Path coverage: test all possible execution paths.</li>
</ul>
<p><strong>3. Experience-based Techniques</strong><br>
Rely on tester’s intuition and experience.</p>
<ul>
<li>Error guessing: Predict likely problem areas based on past defects.</li>
<li>Exploratory testing: Simultaneous learning and test design/execution.</li>
</ul>
<h2 id="static-testing">Static Testing</h2>
<ul>
<li>A software testing technique that involves <strong>reviewing</strong> code, documents, or other project artifacts <strong>without executing</strong> the program.</li>
<li>Aims to identify defects early in the development lifecycle.</li>
</ul>
<h3 id="static-testing-activities">Static Testing activities:</h3>
<ol>
<li>Reviews</li>
</ol>
<ul>
<li>Informal review - Peer feedback without documentation</li>
<li>Walkthrough - Author presents the document for feedback</li>
<li>Technical review - Peer evaluation of technical content. Led by moderator with no management participation</li>
<li>Inspection - Formal process with defined roles(e.g., moderator, reader). Led by moderator and uses entry and exit criteria</li>
</ul>
<h4 id="review-stages">Review Stages</h4>
<ul>
<li>Planning</li>
<li>Kick-off</li>
<li>Review meeting</li>
<li>Rework</li>
<li>Follow-up</li>
</ul>
<ol start="2">
<li>Static Analysis (Automated)</li>
</ol>
<ul>
<li>Code analysis tools check for coding standard violations, security flaws, dead code, etc.</li>
</ul>
<h3 id="artifacts-reviewed-in-static-testing">Artifacts Reviewed in Static Testing:</h3>
<ul>
<li>Requirements documents</li>
<li>Design documents</li>
<li>Source code</li>
<li>Test cases and plans</li>
<li>User manuals</li>
</ul>
<h2 id="functional-design-document-fdd">Functional Design Document (FDD)</h2>
<ul>
<li>A FDD describes how a software system will behave from the user’s perspective.</li>
<li>Defines functional requirements and outlines how the system should function to meet business needs.</li>
<li>Typically written by Business analysts or functional designers.</li>
</ul>
<h2 id="work-breakdown-structure-wbs">Work Breakdown Structure (WBS)</h2>
<p>A WBS is a hierarchical decomposition of a project into smaller, manageable parts.</p>
<h3 id="components-of-wbs">Components of WBS</h3>
<ul>
<li>Work package : Lowest level in WBS where work is defined and estimated</li>
<li>Deliverables : Outputs from each phase</li>
<li>Level : Each tier in the hierarchy</li>
</ul>
<h2 id="stlc">STLC</h2>
<pre><code>Req Analysis &gt; Test planning &gt; Test case development &gt; Test environment setup &gt; Test execution &gt; Test cycle closure
</code></pre>
<ul>
<li>Test plan : formal document outlining strategy, objectives, scope, schedule, resources, activities needed for software testing.</li>
</ul>
<h3 id="sample-defect-report-short-format">Sample Defect Report (Short Format):</h3>
<ul>
<li>
<p><strong>Defect ID</strong>: BUG-102</p>
</li>
<li>
<p><strong>Title</strong>: “Search results do not display relevant items”</p>
</li>
<li>
<p><strong>Severity</strong>: Major</p>
</li>
<li>
<p><strong>Priority</strong>: High</p>
</li>
<li>
<p><strong>Module</strong>: Product Search</p>
</li>
<li>
<p><strong>Environment</strong>: Chrome 115, Windows 11</p>
</li>
<li>
<p><strong>Preconditions</strong>: User logged in</p>
</li>
<li>
<p><strong>Steps to Reproduce</strong>:</p>
<ol>
<li>
<p>Go to homepage</p>
</li>
<li>
<p>Enter “laptop” in the search bar</p>
</li>
<li>
<p>Click Search</p>
</li>
</ol>
</li>
<li>
<p><strong>Actual Result</strong>: Returns unrelated products (e.g., phone cases)</p>
</li>
<li>
<p><strong>Expected Result</strong>: Show relevant laptops</p>
</li>
<li>
<p><strong>Attachments</strong>: [screenshot.png]</p>
</li>
<li>
<p><strong>Status</strong>: New</p>
</li>
<li>
<p><strong>Assigned To</strong>: dev-john</p>
</li>
</ul>

