# Aivora – Product Requirements Document (PRD)

**Document Status:** Initial Draft  
**Product Stage:** Pre-MVP  
**Product Type:** B2B SaaS – Hospitality Technology

## 1. Product Overview

Aivora is an AI-powered hospitality platform designed to automate guest communication and support hotel operations through specialized AI agents.

The initial product will focus on guest inquiries, guest request management, and internal department coordination.

## 2. Product Objectives

The MVP should:

1. Reduce the time spent handling repetitive guest inquiries.
2. Provide consistent guest communication.
3. Capture and organize guest requests.
4. Route requests to the correct hotel department.
5. Give hotel managers visibility into activity and performance.
6. Demonstrate measurable value in a real hotel environment.

## 3. User Roles

### 3.1 Hotel Administrator
- Manage property settings.
- Manage staff accounts and permissions.
- Configure AI assistant behavior.
- View reports and operational activity.

### 3.2 Front Desk Employee
- View guest inquiries.
- Review AI-generated responses.
- Handle requests requiring human attention.
- Update request status.

### 3.3 Department Employee
- Receive assigned tasks.
- Review guest requests.
- Update task progress.
- Mark tasks as completed.

### 3.4 Guest
- Communicate with the hotel through supported channels.
- Ask questions.
- Submit service requests.
- Receive updates and responses.

## 4. Core MVP Modules

### Module 1 – AI Guest Assistant

The AI assistant should:

- Understand guest questions.
- Respond using approved hotel information.
- Support multiple languages.
- Identify the intent of a guest message.
- Escalate uncertain or sensitive requests to hotel staff.
- Maintain relevant conversation context.

### Module 2 – Guest Request Management

The system should:

- Receive guest requests.
- Categorize requests.
- Record request details.
- Assign requests to the appropriate department.
- Track request status.
- Record completion information.

Example categories:

- Housekeeping.
- Maintenance.
- Front Desk.
- Room Service.
- General Inquiry.

### Module 3 – Staff Dashboard

The dashboard should display:

- Total guest requests.
- Pending requests.
- In-progress requests.
- Completed requests.
- Requests requiring human attention.
- Recent guest interactions.

### Module 4 – AI Knowledge Base

Hotel administrators should be able to manage approved information such as:

- Hotel facilities.
- Check-in and check-out policies.
- Restaurant information.
- Frequently asked questions.
- Services and operating hours.
- Hotel policies.

The AI assistant should use this information when generating answers.

### Module 5 – Notifications

The platform should notify relevant staff when:

- A new guest request is received.
- A request is assigned.
- A request requires urgent attention.
- A task remains unresolved.

Notification channels will be selected during technical design.

### Module 6 – Reports and Analytics

The platform should provide:

- Guest inquiry volume.
- Request categories.
- Request completion statistics.
- Response time metrics.
- AI handling and escalation statistics.
- Operational activity summaries.

## 5. Main User Workflow

### Guest Inquiry Workflow

1. A guest sends a message through a supported channel.
2. Aivora receives the message.
3. The AI assistant identifies the guest's intent.
4. The system checks the approved hotel knowledge base.
5. The assistant generates a response.
6. If the request requires action, the system creates a task.
7. The task is routed to the appropriate department.
8. Staff update the task status.
9. The interaction is recorded for reporting.

## 6. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | Secure user authentication | Must Have |
| FR-02 | Property and staff management | Must Have |
| FR-03 | AI guest inquiry handling | Must Have |
| FR-04 | Knowledge base management | Must Have |
| FR-05 | Guest request classification | Must Have |
| FR-06 | Department task assignment | Must Have |
| FR-07 | Request status tracking | Must Have |
| FR-08 | Operational dashboard | Must Have |
| FR-09 | Staff notifications | Should Have |
| FR-10 | Advanced analytics | Should Have |
| FR-11 | Multiple communication channels | Future |
| FR-12 | Hotel PMS integrations | Future / Subject to validation |

## 7. Non-Functional Requirements

### Security
- Secure authentication.
- Role-based access control.
- Secure storage of credentials.
- Encryption in transit.
- Appropriate protection of guest information.

### Performance
- Responsive dashboard experience.
- Reliable processing of guest messages.
- Clear handling of temporary service failures.

### Scalability
- Architecture designed to support multiple hotel properties.
- Separation of each property's data.
- Ability to expand integrations and AI capabilities.

### Reliability
- Logging of important system events.
- Error monitoring.
- Retry handling for supported failed operations.
- Human escalation when AI cannot safely complete a request.

## 8. Human Oversight

Aivora must not autonomously make sensitive commitments or decisions without appropriate authorization.

Examples requiring staff review may include:

- Refunds.
- Booking cancellations.
- Payment disputes.
- Complaints requiring management intervention.
- Special requests outside approved hotel policies.

## 9. MVP Scope Exclusions

The first version will not attempt to provide:

- A complete hotel property management system.
- Full hotel accounting.
- Automated financial transactions.
- Unrestricted autonomous booking changes.
- Every possible third-party integration.

These features may be evaluated in later product phases.

## 10. MVP Success Criteria

The pilot should measure:

- Reduction in repetitive staff workload.
- Guest inquiry response time.
- Accuracy of request classification.
- Successful department routing.
- Percentage of requests completed.
- Staff and management satisfaction.
- Cost of AI usage per property.

Specific performance targets will be established after collecting baseline data from pilot hotels.

## 11. Open Product Decisions

The following decisions must be validated before implementation:

- Which communication channel should be supported first?
- Should the first pilot focus on guest inquiries or operational requests?
- Which hotel PMS or CRM systems are most important?
- Which languages are essential for the initial market?
- What level of human approval should be required for each action?
