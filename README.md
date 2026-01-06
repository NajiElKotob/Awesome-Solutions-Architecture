# Solutions Architecture
{Awesome Works in Progress}

## Solutions Architect
`A solutions architect creates the overall technical vision for a specific solution to a business problem.`
* [What Is a Solutions Architect (and How Do I Become One)?](https://www.coursera.org/articles/solutions-architect?msockid=384df28e91e76f200fc5e7c790ff6e63) - coursera.org
  
## Before We Design Anything!
`Why do software projects fail, and what should we learn before designing a solution?`
* [Software Development Failures](https://direct.mit.edu/books/monograph/3815/Software-Development-Failures) - mit.edu
* [MIT Finds 95% Of GenAI Pilots Fail Because Companies Avoid Friction](https://www.forbes.com/sites/jasonsnyder/2025/08/26/mit-finds-95-of-genai-pilots-fail-because-companies-avoid-friction/) - forbes.com | 2025
* [14 Common Reasons Software Projects Fail (And How To Avoid Them)](https://www.forbes.com/councils/forbestechcouncil/2020/03/31/14-common-reasons-software-projects-fail-and-how-to-avoid-them/) - forbes.com | 2022
* [Survivorship bias](https://www.warhistoryonline.com/war-articles/abraham-wald.html) - warhistoryonline.com

## Business Analysis
`Why is this solution needed, and what business problem does it solve?`
### Business Goals & Success Criteria
* [10 Effective Success Criteria Examples for Successful Projects](https://www.indeed.com/career-advice/career-development/project-success-criteria-examples)

### Requirements Elicitation
* [Elicitation Techniques](https://sites.nd.edu/businessanalysis/?page_id=321)
  - Stakeholder Identification & Analysis – Identifying who the stakeholders are, their roles, influence, and interest.
  - Document Analysis – Review existing documents to understand business context, rules, and constraints.
  - Business Rules & Constraints – Identify policies, regulations, and limitations that shape the solution.
  - Stakeholder Interviews – Gather insights, expectations, and pain points directly from key stakeholders.
  - Observation (Job Shadowing) – Understand real workflows by watching users perform their tasks.
  - Facilitated Workshops – Collaborative sessions to align stakeholders and clarify requirements.
  - Questionnaires & Surveys – Collect structured input from a large audience efficiently.
  - Focus Groups – Gather collective feedback and perspectives from representative users.
  - Brainstorming – Generate ideas and explore possible solution directions.
    - [What is a flowchart?](https://www.youtube.com/watch?v=vBtGO9pXfrQ) - Lucid Software
  - Prototyping (Low-fidelity) – Validate ideas early using simple mockups or sketches.
    - MVP (Minimum Viable Product) - Building a low-cost version of the software with only the core features,
just enough to validate the idea with real users and get feedback.
* → `Requirements elicitation produces raw, unstructured inputs, such as: Business problems, Stakeholder needs, Pain points, Expectations, Constraints mentioned in discussions, Nice-to-haves, Conflicting requests`
-----

## Scope Models
`What is included in the solution, and what is explicitly excluded?`

### Strategic Intent (The "Why")
* Business Objective Model: Usually a diagram showing how high-level problems relate to business value. (Diagram*) → Project Charter & KPI definition
* Goal Model: Text-heavy or a weighted diagram quantifying the objectives. (Text/Diagram*) → Success metric validation (QA/UAT)

### System Boundaries (The "Where")
* Ecosystem Map: A high-level visual of the world around your system. (Diagram) → Identifying integration touchpoints
* Context Diagram:  Shows the system boundary and its interactions with external actors and systems. (Diagram/DFD-0*) → System Architecture & Data Flow design
  - [What is a context diagram? And how to create one (+ examples)](https://www.figma.com/resource-library/context-diagram/) - figma.com
* In-Scope / Out-of-Scope: A definitive T-Chart table. → Change Management & Budgeting

### Process & Functionality (The "What")
* Business Process Scope: Business Process Scope is the clear definition of the boundaries of a business process, specifying where the process starts, where it ends, and what activities, roles, and systems are included or excluded. (Text/Flowchart*) → BPMN
* Feature Model: Feature Model is a structured representation of system or process features. → Functional requirements; Use cases; User stories
* Use Case Diagram: At the scope models phase, the Use Case Diagram is used to clarify who interacts with the system, identify the major system capabilities, and set clear functional boundaries. At this stage, the diagram remains high-level, focusing on overall interactions rather than internal logic; therefore, it is not detailed and not behavioral, and it avoids describing process flows or execution steps. → Detailed use case specifications, BPMN, solution or system design.


### Execution Realities (The "Constraints")
* Assumptions & Dependencies and Constraints: They establish the external conditions, limitations, and guardrails that must be considered, ensuring that process models, system designs, timelines, and budgets remain realistic, feasible, and aligned with agreed boundaries.  → Requirements definition, solution design, project planning, and risk analysis.


### Validation (The "How It Looks")
* Storyboard: A series of frames (sketch or wireframe) showing a user journey. → UX/UI Design & Frontend Development


-----


## Application Analysis
`What must the application do?`
### Process Model
`What activities happen, and in what order?`
* Business processes
  - [What Is a Business Process and How Is It Used?](https://www.coursera.org/articles/business-process?msockid=384df28e91e76f200fc5e7c790ff6e63) - coursera.org
  - [BPMNs in Lucidchart 📺](https://www.youtube.com/watch?v=5Y5TqU8lbRU) - Business Process Model and Notation is a graphical representation for specifying business processes in a business process model. 
* System workflows
  - [What is a workflow?](https://www.ibm.com/think/topics/workflow)
* Use case
  - [How to Make a UML Sequence Diagram 📺](https://www.youtube.com/watch?v=pCK6prSq8aw)
  - [UML use case diagrams 📺 ~13min](https://www.youtube.com/watch?v=4emxjxonNRI) - Lucid Software
  - [Making a use case diagram: How-tos, templates, and tips](https://www.canva.com/online-whiteboard/use-case-diagram/) - canva.com
  - User–system interaction scenarios
* Data Flow Diagrams (DFD)
  - [What is a Data Flow Diagram](https://www.lucidchart.com/pages/data-flow-diagram0) - lucidchart.com


### Rule Model
`What rules govern system behavior?`
* Business rules
* Validation rules
* Decision logic

### Data Model
`What data does the system manage?`
* Entity Relationship Diagram (ERD)
  - Entities
  - Attributes
  - Relationships
* Data Dictionary
* State Table and State Diagram

-----

## Application Design
`How will the application be built?`

### Logical Architecture
`Defines the high-level structure of the system`

* Major components/modules
* Responsibilities of each component
* Layered architecture


### Interaction Design
`Defines how components communicate`

* Component interactions
* Sequence diagrams (high-level)
* Service boundaries

### Design Patterns & Principles
`Defines how problems are solved consistently`

* Architectural patterns (Layered, MVC, MVVM, etc.)
* Design principles (SOLID, separation of concerns)


### Architecture Decisions Records (ADRs)
`Captures why design choices were made`

* Alternatives considered
* Trade-offs
* Final decision

### UI / UX Design
`Defines how users interact with the system`
* UX flows & navigation
* UI guidelines & consistency
* Accessibility considerations
* References
  - [UI/UX](https://goodui.org/) - goodui.org
  - [WinUI 3 Gallery](https://github.com/microsoft/WinUI-Gallery)
  - [Apple Design Resources](https://developer.apple.com/design/resources/) - apple.com
  - [Material Design](https://m3.material.io/)


-----

## Data Architecture
`What data is needed, where does it come from, and how is it structured and stored?`
* Data domains & entities
* Data sources (internal / external)
* Data models (logical / physical)
* Data ownership & governance
* Data quality & lifecycle

-----

## Integration Architecture
`How does the application communicate with other systems and services?`
* Integrated systems & services
* Integration patterns (API, events, files)
* Data exchange & contracts
* Error handling & resilience
  
-----

## Infrastructure & Security
`Where will the application run, and how is it protected and secured?`
* Deployment model & environments
* Hosting & runtime platform
* Identity & access management
* Security controls & compliance
* Availability & resilience

-----

## Architecture & Engineering Reference Frameworks
* [ISO/IEC/IEEE 42010:2022](https://www.iso.org/standard/74393.html)
* [TOGAF (The Open Group Architecture Framework)](https://www.opengroup.org/togaf) - opengroup.org | The TOGAF Standard, a standard of The Open Group, is a proven Enterprise Architecture methodology and framework used by the world’s leading organizations to improve business efficiency.
  - [TOGAF in 10 Minutes 📺](https://www.youtube.com/watch?v=AihWJ3_klRQ) - Software Architecture Monday
* [The Scrum Guide](https://scrumguides.org/scrum-guide.html) - scrumguides.org
* [RACI](https://www.projectmanagement.com/wikis/234008/raci#_) - projectmanagement.com
-----

## Tools
* [miro](https://miro.com/) - miro.com | Get from brainstorm to breakthrough with Miro Where teams and AI ideate, plan, and build the right things faster 
* [Excalidraw](https://excalidraw.com/) - excalidraw.com
* [Lucidchart](https://www.lucidchart.com/) - lucidchart.com
* [Storyboard That](https://www.storyboardthat.com/) - storyboardthat.com
* [Canva](https://www.canva.com/) - canva.com+
* [Visio](https://www.microsoft.com/en-us/microsoft-365/visio/) - Transform the way you use and visualize data to bring your best ideas to life.
* [Figma](https://www.figma.com/) - figma.com | Figma lets you turn big ideas into real products. Brainstorm, design, and build with your team.
  - [Figma Tutorial for Beginners 📺 ~13min](https://www.youtube.com/watch?v=jQ1sfKIl50E)
* [Code Wiki (Google)](https://developers.googleblog.com/en/introducing-code-wiki-accelerating-your-code-understanding/)

-----

## YouTube 📺
* [Software Architecture Monday](https://www.youtube.com/@markrichards5014) - Software Architecture Monday with Mark Richards is a free software architecture channel containing 10 minute videos about some aspect of software architecture.

## Certifications
* [Azure Solutions Architect Expert](https://learn.microsoft.com/en-us/credentials/certifications/azure-solutions-architect/) - microsoft.com
* [PMI Professional in Business Analysis (PMI-PBA)](https://www.pmi.org/certifications/business-analysis-pba) - pmi.org
* [7 Popular Certifications for Solutions Architects](https://www.coursera.org/articles/certifications-for-solutions-architect?msockid=384df28e91e76f200fc5e7c790ff6e63) - coursera.org
