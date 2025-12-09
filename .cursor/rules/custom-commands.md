# Custom Commands/Macros

The following custom commands are available for this project:

## Gen SRS from TC
Generate Software Requirements Specification (SRS) from Truth Criteria (TC) documents.
- **Source:** `/truth/TC.vX.md`
- **Output:** `/requirements/SRS.md`
- **Process:** Extract requirements from truth criteria, ensuring all requirements are traceable to TC with `derived-from:` tags.

## Expand BR from SRS
Expand Business Requirements (BR) from Software Requirements Specification (SRS).
- **Source:** `/requirements/SRS.md`
- **Output:** `/requirements/BR.md`
- **Process:** Derive business requirements from technical SRS, maintaining traceability with `origin:` tags.

## Gen Flows from BR
Generate User Flows and Process Flows from Business Requirements.
- **Source:** `/requirements/BR.md`
- **Output:** `/design/flows/`
- **Process:** Create flow diagrams and descriptions based on business requirements. Include `derived-from: /requirements/BR.md` tags.

## Gen ERD from Flows + BR
Generate Entity Relationship Diagram (ERD) from Flows and Business Requirements.
- **Source:** `/design/flows/` and `/requirements/BR.md`
- **Output:** `/architecture/ERD.md` or `/architecture/ERD.diagram`
- **Process:** Extract entities, relationships, and attributes from flows and business requirements. Tag with `derived-from:` references.

## Gen API from ERD
Generate API specifications from Entity Relationship Diagram.
- **Source:** `/architecture/ERD.md`
- **Output:** `/backend/api/` or `/architecture/API.md`
- **Process:** Design REST/GraphQL endpoints based on ERD entities and relationships. Include `derived-from: /architecture/ERD.md` tags.

## Gen Frontend Component from ComponentContract
Generate Frontend Component code from Component Contract specifications.
- **Source:** Component Contract (typically in `/design/ComponentContract.md` or similar)
- **Output:** `/frontend/components/`
- **Process:** Generate React/React Native components based on contract specifications (props, state, behavior). Include `derived-from:` tags referencing the contract.

