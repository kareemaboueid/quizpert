# Quizpert - Smarter Quizzes for Sharper Hiring

See the [SRS](docs/Quizpert_SRS.md) for more details on the project.

## Description

**Quizpert** is a streamlined, professional-grade tool designed to help recruiters and hiring teams manage technical quizzes during the interview process. Rather than trying to replace the entire recruitment workflow, **Quizpert focuses solely on what matters most in early candidate evaluation**: smart, structured, and consistent quiz-based assessments.

With Quizpert, companies can create, assign, and evaluate multiple-choice quizzes to better gauge candidates' technical knowledge before moving forward in the interview pipeline. From question banks to result analysis, everything is centralized, easy to manage, and purpose-built for interview rounds.

Whether you're hiring engineers, designers, analysts, or other technical roles — Quizpert turns casual quiz sessions into meaningful evaluation data.

> Quizpert is not a full recruitment or applicant tracking system. It specializes exclusively in **interview-related quiz management**.

## Key Features

- **Structured Quiz Management**  
  Create and organize quizzes from a central QA bank. Easily assign quizzes to candidates based on department or role.

- **Auto-Evaluated Results**  
  Once a candidate submits a quiz, Quizpert automatically calculates results and highlights correct vs. incorrect answers.

- **Admin-Controlled User Access**  
  Only recruiters and hiring managers can create and manage users, ensuring full control over who accesses and submits assessments.

- **Detailed Answer Records**  
  Get per-question breakdowns, answer logs, and scoring insights to support hiring decisions and reporting.

## Who Is Quizpert For?

- Recruiters and Hiring Managers  
- HR Departments with technical recruiting needs  
- Department Leads / Engineering Managers  
- Small to Mid-Sized Companies that need lightweight, interview-specific tools

## Technical Overview

**Quizpert** is a full-stack web application optimized for use in structured interview evaluations. It enables Admins (recruiters) to create quizzes, questions, and applicants (users), while applicants can access and submit quizzes securely.

### Core Data Models

- `Admin`: Manages quizzes, users, and QA
- `User`: Takes quizzes, submits answers
- `Quiz`: A set of questions created by Admins
- `QA`: A question/answer bank with correct answers
- `Result`: Submission + scoring of a quiz by a user
- `AnswerRecord`: Detailed answer logs per question

## Tech Stack

| Layer           | Toolset                                                      |
| --------------- | ------------------------------------------------------------ |
| **Frontend**    | React.js, Bootstrap (or React-Bootstrap), Axios              |
| **Backend**     | Node.js, Fastify, Zod/Joi, Prisma ORM, TypeScript (optional) |
| **Database**    | MS SQL Server                                                |
| **Auth**        | JWT-based auth (access & refresh tokens)                     |
| **DevOps**      | Docker, PM2, GitHub Actions (CI/CD), dotenv                  |
| **Testing**     | Jest/Vitest                                                  |
| **Docs & Logs** | Swagger (via Fastify), Winston or Pino logger                |
