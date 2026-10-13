---
layout: page
title: FAQ
permalink: /faq/
description: Biostatistician effort and resource allocation. Guidelines for investigators planning projects and grants with the Biostatistics Core (updated 09/22/25).
nav: true
nav_order: 5.5
---

{%- assign L = site.data.links -%}

<style>
.takeaways { background: #8C1515; color: #fff; border-radius: 12px; padding: 1.5rem 1.75rem; margin: 0 0 2rem; }
.takeaways h3 { color: #fff !important; margin: 0 0 .75rem; font-size: 1.2rem; }
.takeaways ol { margin: 0; padding-left: 1.25rem; }
.takeaways li { color: #fff; margin: .3rem 0; }
.faq-intro { margin-bottom: 1.5rem; }
.faq-section { margin: 2.25rem 0 0; }
.faq-section > h2 { font-size: 1.45rem; padding-bottom: .35rem; border-bottom: 2px solid #8C1515; margin-bottom: 1rem; }
.faq-section details { border: 1px solid var(--global-divider-color); border-radius: 8px; margin: 0 0 .6rem; background: var(--global-bg-color); }
.faq-section summary { cursor: pointer; padding: .85rem 1.1rem; font-weight: 600; list-style: none; position: relative; padding-right: 2.5rem; }
.faq-section summary::-webkit-details-marker { display: none; }
.faq-section summary::after { content: "+"; position: absolute; right: 1.1rem; top: .7rem; font-size: 1.3rem; color: #8C1515; }
.faq-section details[open] summary::after { content: "–"; }
.faq-section details[open] summary { border-bottom: 1px solid var(--global-divider-color); }
.faq-section .answer { padding: .9rem 1.1rem .4rem; }
.faq-section .answer p, .faq-section .answer li { line-height: 1.6; }
.effort-wrap { overflow-x: auto; margin: 1rem 0 1.5rem; }
.effort { width: 100%; border-collapse: collapse; font-size: .92rem; min-width: 640px; }
.effort th, .effort td { border: 1px solid var(--global-divider-color); padding: .55rem .7rem; text-align: center; vertical-align: middle; }
.effort thead th { background: #8C1515; color: #fff; }
.effort tbody th { text-align: left; background: rgba(140,21,21,.06); }
.tiers { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 1rem; margin: 1rem 0; }
.tier { border: 1px solid var(--global-divider-color); border-top: 4px solid #8C1515; border-radius: 10px; padding: 1.1rem 1.2rem; }
.tier h4 { margin: 0 0 .25rem; font-size: 1.1rem; }
.tier .pct { font-weight: 700; color: #8C1515; margin: 0 0 .6rem; }
.tier p.lbl { font-weight: 600; margin: .7rem 0 .25rem; font-size: .9rem; }
.tier ul { padding-left: 1.1rem; margin: 0; font-size: .9rem; }
.tier li { margin: .2rem 0; }
.footnotes-small { font-size: .85rem; color: var(--global-text-color-light); }
</style>

<p class="faq-intro">These FAQs were developed by the Nephrology Division Biostatistics Core as guidelines for investigators to understand the value of including a biostatistician team in their projects and what that collaboration entails. Details on effort allocation are based on other Biostatistics Centers.</p>

<div class="takeaways">
<h3>Top 5 take-home points</h3>
<ol>
<li>Biostatisticians play a vital role in research!</li>
<li>Engage with a biostatistician at least <strong>8 weeks</strong> before a grant is due.</li>
<li>Include funding for biostatistician(s) effort in all grant proposals.</li>
<li>Include biostatisticians as co-authors on papers where appropriate.</li>
<li>Biostatistician effort will also include time devoted to methods development and accompanying methods-focused manuscripts germane to the project when appropriate.</li>
</ol>
</div>

<section class="faq-section">
<h2>The benefits of including a biostatistician</h2>

<details open>
<summary>1. Why is it crucial to involve biostatisticians in research projects?</summary>
<div class="answer">
<p>Biostatisticians play a vital role in research, ensuring that:</p>
<ul>
<li>Study objectives are clearly defined and testable.</li>
<li>Study designs are efficient and aligned with objectives.</li>
<li>Data is collected and documented appropriately.</li>
<li>Proper statistical analyses are conducted and accurately reported.</li>
</ul>
<p>Their expertise in translating scientific hypotheses into actionable analyses, combined with their knowledge of innovative methods from various disciplines, strengthens the research proposal, increases the likelihood of funding, and enhances the impact of the research.</p>
</div>
</details>

<details>
<summary>2. When should I consult with a biostatistician during the grant proposal process?</summary>
<div class="answer">
<p>Engage a biostatistician <strong>at least 8 weeks before the proposal due date</strong>. Early involvement allows them to contribute effectively to:</p>
<ul>
<li><strong>Brainstorming ideas.</strong> Researchers have found that involving a statistician very early in the inception of the project increases grant success.</li>
<li>Defining research objectives and approach.</li>
<li>Writing the proposal, especially the statistical analysis section.</li>
</ul>
</div>
</details>

<details>
<summary>3. How do I include a biostatistician in my research project and grant proposal?</summary>
<div class="answer">
<p>Fill out a support request to the Division of Nephrology Biostatistics Core using the <a href="{{ L.support_request_form }}">Project/Grant Support Request Form</a>. You will be asked to submit a draft protocol when requesting support for a project (see question 7). A <a href="{{ L.protocol_template }}">protocol template</a> is available.</p>
</div>
</details>

<details>
<summary>4. Do I need to pay for the statistician's time in writing a grant proposal?</summary>
<div class="answer">
<p>Biostatisticians often contribute to proposal development (e.g., power calculations, writing statistical sections) without initial compensation, anticipating funded effort post-award. Conversations need to occur to determine the appropriate budget for biostatistician and programmer effort, software, and other resources to be included in the grant budget.</p>
</div>
</details>

<details>
<summary>5. What factors determine authorship for biostatisticians?</summary>
<div class="answer">
<p>Authorship is based on contributions, not financial considerations. A biostatistician should be considered a co-author if they substantially contribute to either study design or data analysis and interpretation <em>and</em> participate in drafting or revising the manuscript. Please see the <a href="https://www.icmje.org/recommendations/browse/roles-and-responsibilities/defining-the-role-of-authors-and-contributors.html">ICMJE recommendations</a> for more details. Research has demonstrated that including a biostatistician on a grant application or manuscript improves chances for funding and publication.</p>
</div>
</details>

<details>
<summary>6. What timelines need to be considered at a project's outset?</summary>
<div class="answer">
<p>The team must discuss the overall project timeline, considering factors such as the fellow's clinic schedule and research time, the statistician's availability, and potential delays like data availability or IRB approvals. Clear deadlines should be established to ensure the Biostatistics Core team can adequately plan and support the project.</p>
</div>
</details>

<details>
<summary>7. What is the importance of an analysis plan/protocol and where can I find a template?</summary>
<div class="answer">
<p>An analysis plan, outlining the statistical approach aligned with the research question, is crucial. The entire team must approve this plan before analysis begins. This ensures everyone understands the methods used and helps avoid potential misinterpretations. The Biostatistics Core created a general <a href="{{ L.protocol_template }}">protocol template</a> that should be submitted by researchers when requesting support (see question 3). Once the project starts, a full protocol will be developed by the entire research team.</p>
</div>
</details>
</section>

<section class="faq-section">
<h2>Effort allocation</h2>

<details open>
<summary>1. How is the effort allocation for a biostatistician determined?</summary>
<div class="answer">
<p>Effort allocation, expressed as a percentage, is described in <a href="#table1">Table 1</a>. These are meant as guidelines, and appropriate allocation should be discussed with the Biostatistics Core during grant development. Effort allocation should include time devoted to methods development and associated methods manuscripts germane to the specific aims of the grant. Methods publications enhance the productivity of the grant by demonstrating teamwork, strengthening statistical prowess, and increasing publications included in yearly reports submitted to the funding agency.</p>
</div>
</details>

<details>
<summary>2. What are the different effort levels for biostatisticians, and what types of projects do they correspond to?</summary>
<div class="answer">
<p>Effort levels and corresponding project types are displayed in <a href="#table1">Table 1</a> below. These are meant as guidelines, and appropriate efforts should be determined by the Biostatistics Core during grant development.</p>
</div>
</details>

<details>
<summary>3. Can the allocated biostatistician effort be adjusted after the grant is funded?</summary>
<div class="answer">
<p>No, adjusting biostatistician effort without prior approval and justification is not acceptable. Any budget changes affecting their effort must be discussed and agreed upon by the PI, the Biostatistics Core, and the finance team. If budget cuts necessitate effort reduction, the scope of the work must also be adjusted accordingly. Similarly, if the scope of the project increases, the budget for the biostatistics team should increase accordingly.</p>
</div>
</details>

<details>
<summary>4. Are there any funding sources for biostatistician effort on unfunded projects?</summary>
<div class="answer">
<p>Limited support may be available. This needs to be discussed with the finance team and Division Chief.</p>
</div>
</details>

<details>
<summary>5. What are some additional budgetary considerations for biostatistician involvement?</summary>
<div class="answer">
<p>The PI and lead biostatistician should have a conversation while drafting the budget about the needs of the biostatistician team to complete the project. This may include additional resources, like specialized software, publication costs, training specific to the project needs, or conferences.</p>
</div>
</details>
</section>

<section class="faq-section">
<h2>Training grants</h2>

<details open>
<summary>1. Can a biostatistician mentor be included in K Awards and other training grants?</summary>
<div class="answer">
<p>Having a biostatistician mentor on K awards and other training grant mechanisms is often needed for the success of the award. These mechanisms generally do not support funded effort for biostatistician faculty. In this case, the PI should discuss the proposal with the Division Chief. Effort may be suitably budgeted for a staff biostatistician to conduct the programming and analytic work needed for the project that is not part of the mentoring plan.</p>
</div>
</details>

<details>
<summary>2. Who should be included in every fellowship research project team?</summary>
<div class="answer">
<p>Any project request submitted to the Biostatistics Core to support a fellow's research must include a faculty mentor. A senior statistician plus an analyst statistician, if needed, will be assigned to the project.</p>
</div>
</details>

<details>
<summary>3. What are the responsibilities and expectations for each member in a fellowship research project team?</summary>
<div class="answer">
<p>The team must collectively agree on the project goals, including the number of publications and grant applications. Open communication and regular meetings are crucial for a successful collaboration. Expectations are as follows:</p>
<ul>
<li><strong>The fellow</strong> drives the project, understanding the data and ensuring appropriate clinical interpretation.</li>
<li><strong>The faculty mentor</strong> guides the research direction and oversees the fellow's progress. The mentor actively participates in defining the research question, stays updated on project progress, provides feedback to the fellow and team, and ensures the project's completion even if the fellow graduates before the project concludes.</li>
<li><strong>The senior statistician</strong> oversees the analysis and provides statistical expertise.</li>
<li><strong>The analyst</strong> (if included) performs the statistical programming or supports the fellow by troubleshooting and helping with code creation.</li>
</ul>
</div>
</details>
</section>

<section class="faq-section" id="table1">
<h2>Table 1. Annualized biostatistics effort allocation guidelines<sup>1,2</sup></h2>

<div class="effort-wrap">
<table class="effort">
<thead><tr><th></th><th>Large / complex</th><th>Regular</th><th>Simple</th><th>Basic</th><th>Initial consultation<br><small>(division funded)</small></th></tr></thead>
<tbody>
<tr><th>Total effort</th><td>50–100%+ per year</td><td>30–65% per year</td><td>15–35% per year</td><td>5–15% per year</td><td>1–2 hours</td></tr>
<tr><th>Lead biostatistician</th><td>20%+ per year</td><td>10–15% per year</td><td>5–&lt;10% per year</td><td>0–5% per year</td><td>1–2 hours</td></tr>
<tr><th>Analysis biostatistician</th><td>30–100%+ per year</td><td>20–50% per year</td><td>10–25% per year</td><td>5–10% per year</td><td>0</td></tr>
</tbody>
</table>
</div>

<div class="tiers">
<div class="tier">
<h4>Large / complex projects</h4>
<p class="pct">50–100%+ total effort per year</p>
<p class="lbl">Activity scope</p>
<ul>
<li>Large or complex projects requiring a high level of involvement in development, implementation and communication of results.</li>
<li>Development and/or implementation of complex study designs.</li>
<li>Assembly of datasets from large, complex or poorly documented sources (e.g., administrative or survey databases) or through primary data collection.</li>
<li>Interim data analyses during the data collection phase of prospective studies.</li>
<li>Development and/or use and interpretation of novel or complex statistical methods, with support for publication.</li>
<li>Active participation in publications, with opportunity for first-authored papers.</li>
<li>Regular meetings with PI and collaborators, and separately with the statistical team.</li>
</ul>
<p class="lbl">Examples</p>
<ul><li>R01s, P, U, large team science projects, such as large prospective cohort studies or trials that also include substantial retrospective or record data collection.</li></ul>
</div>
<div class="tier">
<h4>Regular projects</h4>
<p class="pct">30–65% total effort per year</p>
<p class="lbl">Activity scope</p>
<ul>
<li>Standard study designs and routine analyses.</li>
<li>Collaboration through all phases of the study, including attending regular study meetings.</li>
<li>Involvement in study design, implementation and data collection.</li>
<li>Well-documented, established datasets (USRDS, SRTR, STARR) provided for analysis.</li>
<li>Analyses using off-the-shelf procedures in statistical software.</li>
<li>Regular meetings with the PI and collaborators.</li>
<li>Active participation in 3–4 publications, with opportunity for first-authored papers.</li>
</ul>
<p class="lbl">Examples</p>
<ul><li>Most R01s with proposed study design and statistical methods that statisticians would consider standard or routine.</li></ul>
</div>
<div class="tier">
<h4>Simple projects</h4>
<p class="pct">15–35% total effort per year</p>
<p class="lbl">Activity scope</p>
<ul>
<li>Minimal Biostatistician 3 or higher (lead biostatistician) collaboration; straightforward analyses performed by an MS biostatistician (analysis biostatistician).</li>
<li>Occasional meetings with the PI about study issues, such as choice of statistical methods. This level of effort is typically too low for a Biostatistician 3 to carry out analyses or attend weekly meetings.</li>
<li>Generally not compatible with smooth workflows unless an experienced, capable MS biostatistician is adequately supported on the project.</li>
<li>Feedback on 1–2 manuscripts.</li>
</ul>
<p class="lbl">Examples</p>
<ul><li>Smaller-scope R-level grants, such as R21s or fellows' grants.</li></ul>
</div>
<div class="tier">
<h4>Basic projects</h4>
<p class="pct">5–15% total effort per year</p>
<p class="lbl">Activity scope</p>
<ul>
<li>An experienced, capable MS biostatistician is adequately supported and can conduct the study with minimal lead biostatistician involvement.</li>
<li>Occasional meetings between the PI and the analysis biostatistician.</li>
<li>Lead biostatistician meets only with the analysis biostatistician to guarantee quality of results.</li>
<li>Standard analyses on pre-existing, well-documented datasets.</li>
<li>Feedback only on the directly related manuscript.</li>
</ul>
<p class="lbl">Examples</p>
<ul>
<li>Fellows' projects funded with division funds.</li>
<li>Analysis of a single, well-curated dataset for a specific abstract or small paper.</li>
<li>Projects where the PI provides a clean, analysis-ready dataset and requires a single, standard analysis.</li>
</ul>
</div>
<div class="tier">
<h4>Initial consultation</h4>
<p class="pct">1–2 hours (division funded)</p>
<p class="lbl">Activity scope</p>
<ul>
<li>Feedback or advice on a project.</li>
<li>Office hours to discuss a potential project.</li>
<li>Initial grant development discussion.</li>
<li>Defining the scope of a potential project.</li>
</ul>
<p class="lbl">Examples</p>
<ul><li>Consultation-basis work, such as smaller foundation grants, or R-level grants in the basic sciences for which data analysis is not the biostatistician's responsibility.</li></ul>
</div>
</div>

<p class="footnotes-small"><sup>1</sup> Adopted from University of California Davis School of Medicine <em>Guidelines for Estimating Biostatistician Effort and Resource Guidelines on Grants</em> and Northwestern University Feinberg School of Medicine <em>Annualized Biostatistics Effort Allocation Guidelines</em>, except for the description of Basic Projects.<br>
<sup>2</sup> Effort allocation guidelines assume that other necessary resources, such as research study coordinators and project coordinators, are also included in the budget. If a project has a strong research study coordinator or team of coordinators, biostatistics effort may be at the lower end of the range provided (e.g., if the project coordinator sets up and maintains the study database with limited input from the biostatisticians). Notably, biostatistics effort does not include data entry.</p>
</section>

<p style="margin-top:2rem">Ready to start? <a href="{{ L.support_request_form }}">Submit a support request</a> or bring your questions to <a href="{{ L.office_hours_signup }}">office hours</a>.</p>
