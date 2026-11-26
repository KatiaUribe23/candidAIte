# CandidAIte project journal

## November 23, 2026 — Getting started

**Objective.** Start the ethics project in Katia's existing GitHub repository and document its development in English.

**Work completed.** Katia shared the repository and product proposal. Codex reviewed the proposal, opened the repository, and verified that its main branch contained a README. At Katia's request, Codex added this journal and linked it from the README.

**Design discussion.** We discussed a possible demo using a fictional résumé and job posting. An applicant could preview the skills an employer would see, and an employer could review potentially biased wording. Showing how the job fits the applicant's preferences would also give the applicant a voice in the matching process.

**Current state.** The journal is the first project addition. The website and the proposed demo are still at the planning stage.

## November 23, 2026 — Brand identity and first interactive demo

Katia supplied the logo reference, slogan, palette, and typography. Codex sampled the four palette colors and built a responsive Spanish-language prototype with a text-based wordmark. The candidate can edit a fictional project and approve what the employer sees. The employer view displays the approved project and skills. Sharing lasts for the current page session.

A script-level check exercised both views and confirmed that approval displays the edited project. Visual browser testing is pending. The prototype uses a fixed sample and does not yet process uploaded CVs.

Katia reviewed the first version and wanted more depth. Codex added a technical illustration of the sample gripper, individual skill selection, and a way to withdraw a shared profile. A script-level check verified that approval copies the selected skills and edited text, and that withdrawal clears the employer view. The browser test could not launch Edge in this session.

## November 23, 2026 — Page-by-page planning

Katia shared the original project discussion. We reviewed the team's aim to reduce bias linked to school and gender, and the idea of matching jobs and applicants in both directions. The proposed next page is CV intake, leading into the existing candidate review. Later pages will cover vacancy review and explainable recommendations. This entry records planning only.

## November 23, 2026 — Multi-tab recruitment prototype

Katia requested a more developed site with separate workspaces. Codex built five main sections and linked candidate intake, consent, vacancy editing, a rule-based Spanish wording audit, and two illustrative fit indicators. PDF and DOCX selection is local; users enter their own project details manually. Sharing lasts for the open page session.

Script checks covered navigation targets, wording flags, skill and modality calculations, and withdrawal. Visual verification in the in-app browser was blocked for the local file URL.

## November 23, 2026 — Public classroom demo

At Katia's request, Codex published the multi-tab prototype through GitHub Pages using the gh-pages branch. An unauthenticated HTTP request returned status 200 and confirmed the candidate workspace and compatibility section in the published HTML. Demo URL: https://katiauribe23.github.io/candidAIte/

## November 25, 2026 — Mutual compatibility scoring and anonymous talent comparison

Marian updated the matching engine and employer talent view in `index.html` to align the prototype with Sections 6.5 and 7.2 of the Final Product Proposal.

The matching module now calculates a combined mutual compatibility score using the geometric mean ($\sqrt{\text{Employer fit} \times \text{Candidate fit}}$) alongside separate employer and candidate indicators, plus an explicit breakdown of matched and missing skills. In addition, the employer talent section was expanded from a single-profile preview into a structured anonymous comparison across three fictional profiles (`#0084`, `#0127`, and `#0042`), keeping names, photographs, and university prestige hidden.

A code-level review verified valid JavaScript syntax, consistent Spanish UI labels across the prototype, and proper score recalculation when preferred and offered work modalities differ.

## November 26, 2026 — Classroom demo with Marian’s contributions

Marian implemented the three-profile anonymous comparison and geometric-mean compatibility score. Codex published her work to GitHub Pages, added a fictional-CV entry point, corrected the comparison layout, and clarified what happens when a vacancy has no required skills. Script checks covered the three profiles, a 71% mutual fit for a modality mismatch with full skill coverage, missing requirements, and withdrawal. The public URL returned HTTP 200 with the new demo entry point.
