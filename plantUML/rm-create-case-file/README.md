# RM - Create Draft Casefile E2E Interactions

The following UML sequence diagrams illustrate the main backend interactions in the RM Create Draft Casefile journey. They are presented in the order in which each interaction first appears in the frontend journey. UI-only interactions are not shown.

## Get Countries

**Triggered from Respondent Details:** When the page opens, the frontend retrieves active Countries from RM, with United Kingdom presented first. Other address pages reuse this interaction.

## Get Central Authorities

**Triggered from Central Authority Details:** When the optional page opens, the frontend retrieves active Major Creditor records identified as Central Authorities. The page presents their identity, address, Country and contact information for selection.

## Get Maintenance Applications

**Triggered from Order Details:** When the page opens, the frontend retrieves active Maintenance Applications for the Create Casefile application group. The page presents each application code and title for selection.

## Get Results

**Triggered from Order Terms Selection:** When the page opens, the frontend retrieves active Results for the selected Result Type. The page presents each Result code and title for selection.

## Get Result

**Triggered from Order Terms Selection:** When the inputter selects a Result code, the frontend retrieves its complete definition, including `result_parameters`. The returned metadata builds the fields, options, hints and validation on the Order Terms Input page.

## Create Draft Casefile

**Triggered from Check Case Details:** When the inputter selects **Submit for Review**, the frontend submits the Business Unit, Casefile and Casefile Type to RM.
