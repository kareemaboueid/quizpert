# Software Requirements Specification (SRS) for Quizpert

## 1. Functional Requirements

### 1.1 Admin Functionalities

- Create quizzes and manage a bank of questions and answers.
- Add new users using ID/Iqama number without passwords.
- Create departments and associate quizzes with them.
- View analytics and detailed reports.

### 1.2 User Functionalities

- Take quizzes as part of the interview process.
- View their score and performance analytics post-submission.

### 1.3 System Workflows

#### 1. Admin Setup Phase

- Admin logs in and is associated with a department.
- Admin creates a QA bank (questions and answers).
- Admin creates and configures a quiz (title, duration, active status).

#### 2. User Preparation Phase

- Admin adds users under a department.
- Users receive quiz access via links or notifications.

#### 3. Quiz-Taking Phase

- Users log in and start assigned quizzes.
- Each question has multiple-choice answers.
- Users complete and submit the quiz.

#### 4. Result Generation Phase

- System records user answers.
- Scores are calculated and stored.
- Results reflect correct and incorrect answers.

#### 5. Review & Evaluation Phase

- Admin reviews results and user performance.
- Admin adds evaluation notes or flags users for follow-up.

#### 6. Post-Quiz Management

- Data is stored for auditing and future analysis.
- Admins can export reports and improve question banks.

### 1.4 Role-Based Access Control

- Admin: Full access to all system functionalities.
- User: Limited access to quizzes and personal results.
- Developer: Maintenance access (optional).

### 1.5 Quiz Rules

- Time-limited quizzes.
- Scoring enabled.
- Up to three retries, granted manually by admin.
- Quizzes are individually assigned and stored for reuse.

---

## 2. Non-Functional Requirements

- Expected usage: 2 users per week on average; no concurrent usage expected.
- Average performance targets; no high-speed guarantees required.
- No high availability required.
- Strong input validation, sanitization, and encryption required.
- Accessibility support not required.
- Arabic is the default language; localization may be added if needed.
- Basic data integrity and audit logging required.

---

## 3. External Interface Requirements

- Web-based system accessed via browser on desktop or mobile.
- No integrations with external systems (e.g., HR, Slack).
- No APIs required at this stage.
- Separate interfaces for admins and users.
- No email or external communication channels required.

---

## 4. System Constraints

- Confirmed tech stack: Node.js, Fastify, React, MS SQL Server, etc.
- Deployment planned via Hostinger or similar services.
- Licensing and costs based on hosting and developer rates.
- No support required for low-connectivity environments.
- No legal or compliance standards are currently applicable.

---

## 5. Assumptions and Dependencies

- Users will have a clear goal when accessing the system.
- Minimal or no reliance on third-party services or tools.
- No external teams or contractors involved in development.
- Infrastructure limited to MS SQL Server and standard hosting.
- Backup and disaster recovery not a current priority.

---

## 6. Benefits of the SRS

- Aligns project goals with stakeholder expectations.
- Facilitates smoother handoffs to development and QA teams.
- Acts as a reference document throughout the project lifecycle.
- Aids in structured, consistent, and maintainable development.

---

## 7. Clear Communication

- Primary stakeholders: Internal managers and recruiters.
- Sign-off authority: CFO.
- Point of contact for updates: CEO or account manager.

---

## 8. Reduced Development Time and Cost

- Scope and requirements clearly defined to avoid ambiguity.
- Major concern is cost feasibility and stakeholder approval.

---

## 9. Improved Quality and Reliability

- Benchmarks: Completeness, Consistency, Traceability, No Critical Bugs.
- Unit testing will be applied.
- System validation through stakeholder review and test case verification.

---

## 10. Effective Project Management

- Timeline: MVP in 1–2 weeks; additional phases within another 1–2 weeks.
- Project tracking via lightweight tools (e.g., Notion, GitHub Projects).
- The developer (owner) will manage the backlog and priorities.
