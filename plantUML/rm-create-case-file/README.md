# RM - Create Draft Casefile E2E Interactions

The following UML sequence diagrams illustrate the main backend interactions in the RM Create Draft Casefile journey. They are presented in the order in which each interaction first appears in the frontend journey. UI-only interactions are not shown.

## Get Countries

**Called by the Respondent Details, Applicant Details and Minor Creditor Details pages:** Each page requests active Countries for its address fields and lists the United Kingdom first.

## Get Central Authorities

**Called by the Central Authority Details page:** It requests active Major Creditors marked as Central Authorities, then shows their names, addresses and contact details.

## Get Major Creditors

**Called by the Creditor page:** When the inputter chooses the Major Creditor option, the page requests active Major Creditors and shows them for selection.

## Get Maintenance Applications

**Called by the Order Details page:** It requests active Maintenance Applications for Create Casefile, then shows each application code and title.

## Get Results

**Called by the Order Terms Selection page:** It requests active Results that can be used as Order Terms, then shows each Result code and title.

## Get Result

**Called by the Order Terms Input page:** After the inputter selects an Order Term, the page requests its Result metadata and uses `result_parameters` to build the form.

## Create Draft Casefile

**Called by the Check Case Details page:** When the inputter selects **Submit for Review**, the page sends the Business Unit, Casefile and Casefile Type to RM.
