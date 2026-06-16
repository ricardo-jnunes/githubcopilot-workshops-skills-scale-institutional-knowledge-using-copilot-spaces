# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Supporting & Cross-cutting Roles

The following roles support core delivery and ensure quality, security, compliance, and customer success across project execution.

### Release Engineer / Release Manager

**Role Summary**  
Release Engineers own the deployment pipeline, automate release processes, and ensure smooth, safe transitions to production. They work closely with developers, QA, and product teams to coordinate releases and manage rollback strategies.

**Responsibilities**
- Own and maintain release pipelines and deployment automation
- Manage rollback plans and coordinate release validations
- Coordinate pre-release checks with Security and Observability leads
- Document release procedures and runbooks
- Triage and resolve deployment-related issues

**Interactions**
- Works with Developers to understand code changes and dependencies
- Coordinates with QA to ensure all testing gates pass before release
- Partners with PM/PdM to schedule releases and communicate timelines
- Collaborates with Security Engineer on security pre-deployment checks
- Works with Observability Lead to set up post-deploy monitoring and alerts

**Goals**
- Minimize deployment risk and time-to-production
- Achieve zero-downtime or low-impact releases
- Maintain clear release documentation and incident response playbooks

---

### Security Engineer (AppSec)

**Role Summary**  
Security Engineers perform threat modeling, review security findings, and guide teams on secure coding practices. They approve security-related changes and manage vulnerability remediation timelines.

**Responsibilities**
- Perform threat modeling and security architecture reviews
- Review security findings and approve security-related code changes
- Manage vulnerability remediation timelines and escalations
- Define and audit compliance controls
- Provide security guidance to developers and other teams

**Interactions**
- Partners with Developers and QA on security fixes and test strategies
- Advises PdM/PM on security risk trade-offs and business impact
- Escalates critical vulnerabilities to Sponsor when business-impacting
- Collaborates with Compliance/Legal on regulatory requirements
- Works with Release Engineer on pre-deployment security checks

**Goals**
- Minimize security vulnerabilities in delivered features
- Ensure secure-by-design practices across the organization
- Maintain compliance with applicable standards and regulations

---

### Observability / Monitoring Lead

**Role Summary**  
The Observability Lead defines SLOs, sets up dashboards and alerts, and drives post-deploy verification. They create incident triage runbooks and ensure teams have visibility into system health and performance.

**Responsibilities**
- Define SLOs, metrics, and key signals for monitoring
- Set up dashboards, alerts, and observability infrastructure
- Drive post-deploy verification and smoke tests
- Create and maintain incident triage and response runbooks
- Work with teams to instrument code for observability

**Interactions**
- Collaborates with Developers to instrument code and define key metrics
- Works with Operations to set up monitoring and alert infrastructure
- Partners with PM and PdM to track success metrics and dashboards
- Supports Release Engineer with post-deployment verification
- Assists Project Manager in identifying and escalating production issues

**Goals**
- Provide real-time visibility into system health and performance
- Enable fast incident detection and response
- Support data-driven decision-making through metrics and dashboards

---

### Technical Writer / Documentation Owner

**Role Summary**  
Technical Writers maintain user-facing documentation, release notes, runbooks, and internal process documentation. They work with teams across the organization to ensure clarity and consistency.

**Responsibilities**
- Maintain user-facing feature documentation and help articles
- Write and update release notes and migration guides
- Create and manage internal runbooks and process documentation
- Collaborate with teams to keep docs current and accurate
- Organize documentation in `docs/` and `.copilot/` directories as needed

**Interactions**
- Collaborates with PdM for feature descriptions and user-facing content
- Works with Developers for implementation details and technical accuracy
- Partners with PM for release notes and stakeholder communication
- Supports Support/Customer Success with troubleshooting documentation
- Contributes to process documentation and team onboarding materials

**Goals**
- Reduce support volume through clear, discoverable documentation
- Improve onboarding speed and reduce dependency on tribal knowledge
- Maintain a single source of truth for product and process information

---

### Customer Success / Support Liaison

**Role Summary**  
The Support Liaison surfaces customer feedback, pilots releases with early customers, and owns post-release customer communications. They bridge the gap between customers and the product team.

**Responsibilities**
- Surface customer feedback, feature requests, and pain points
- Pilot-test new releases with select customers before broad rollout
- Own post-release customer communications and announcements
- Coordinate with QA on customer-relevant acceptance scenarios
- Triage and escalate customer-impacting issues

**Interactions**
- Feeds feature feedback and customer insights to PdM for backlog prioritization
- Coordinates with PM for stakeholder updates and release communication
- Works with QA to ensure acceptance criteria address real customer workflows
- Collaborates with Technical Writer on user-facing documentation
- Escalates critical customer issues to Project Manager for prioritization

**Goals**
- Maximize customer satisfaction and adoption of new features
- Reduce time-to-value for customers with new releases
- Build strong customer relationships and reduce churn

---

### Data Analyst / Measurement Lead

**Role Summary**  
Data Analysts define instrumentation strategies, produce analytics and dashboards, and measure success metrics. They enable data-driven decision-making across the organization.

**Responsibilities**
- Define event instrumentation and data collection strategies
- Produce dashboards and analytics to measure success metrics
- Analyze experiments and A/B tests to inform product decisions
- Track key performance indicators (KPIs) and business metrics
- Provide insights to support PM and PdM prioritization

**Interactions**
- Works closely with PdM to define success metrics and KPIs
- Collaborates with Developers on instrumentation implementation
- Partners with PM on reporting cadence and stakeholder communication
- Works with Observability Lead to align on key metrics and dashboards
- Supports retrospectives with data on sprint velocity, cycle time, and outcomes

**Goals**
- Enable data-driven decision-making across product and delivery teams
- Provide clear visibility into feature adoption and business impact
- Support continuous improvement through measurement and analysis

---

### Compliance / Legal Liaison

**Role Summary**  
The Compliance Liaison reviews requirements for regulatory compliance, approves data handling practices, and advises on contractual obligations. They ensure projects meet legal and regulatory standards.

**Responsibilities**
- Review requirements for regulatory compliance (GDPR, SOC2, etc.)
- Approve data handling practices and privacy controls
- Advise on contractual obligations affecting releases and deployments
- Audit and document compliance controls
- Escalate compliance risks to leadership

**Interactions**
- Engages with PdM/PM for risk acceptance and compliance trade-offs
- Coordinates with Security Engineer on controls and audit requirements
- Works with Data Analyst on data governance and privacy practices
- Collaborates with Product teams on feature-specific compliance needs
- Escalates high-risk compliance issues to Sponsor

**Goals**
- Ensure all projects and releases meet legal and regulatory requirements
- Minimize compliance risk and audit findings
- Build trust with customers through transparent compliance practices

---

### Delivery Lead (if separate from PM)

**Role Summary**  
When separate from the Project Manager, the Delivery Lead coordinates cross-team dependencies, manages delivery-level scheduling, and runs the day-to-day execution cadence. They focus on removing blockers and keeping teams moving.

**Responsibilities**
- Coordinate cross-team dependencies and integration points
- Manage delivery-level scheduling and sprint execution
- Run daily standups, planning, and retrospective ceremonies
- Identify and escalate blockers using the blocker escalation path
- Maintain delivery dashboards and progress tracking

**Interactions**
- Works alongside PM and Engineering Managers to unblock teams
- Escalates blockers per the escalation path (Team → PM → Product Lead → Sponsor)
- Collaborates with all delivery team members on planning and execution
- Supports Project Manager in maintaining project status and communications
- Partners with Product Manager on backlog readiness and acceptance criteria

**Goals**
- Maintain steady delivery pace and reduce blocker resolution time
- Ensure clear communication and escalation across teams
- Support team autonomy while providing structure and accountability

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When organizing projects, assign clear ownership to one or more personas based on team structure.
- Reference these personas when creating checklists, communication templates, and process artifacts to clarify responsibility.
