# Developer Assessment: Authentication Experience

## Overview

A new software company is launching its first web application and needs an authentication experience. Your task is to design and implement three pages:

1. Login
2. Sign up
3. Forgot password

We want to see how you turn a simple brief into a polished, usable interface and how you structure your frontend code. The backend can be mocked; no real authentication service is required.

## Time and scope

- Aim to spend **4–6 hours** on this assessment. Please stop at six hours and document any unfinished work.
- Use a frontend stack you are comfortable with. Explain your choice briefly in the README.
- You may use UI libraries, icons, and other dependencies. Identify them in the README.
- Choose a temporary company name and a simple visual identity. A separate logo or design file is not required.
- Focus on the three requested pages. Additional features are not required and will not earn extra credit.

## Required pages

### 1. Login

Include:

- Email address and password fields.
- A show/hide password control.
- A login button.
- Links to the sign-up and forgot-password pages.
- Validation for required fields and email format.
- A loading state while the mock request runs.
- Clear feedback for incorrect credentials and successful login.

After successful login, display a simple confirmation state. You do not need to build a dashboard.

### 2. Sign up

Include:

- Full name, email address, password, and confirm-password fields.
- A sign-up button.
- A link back to login.
- Validation for required fields, email format, and matching passwords.
- A visible password rule: **at least eight characters**. Use this rule for the assessment; you do not need to design a production password policy.
- A loading state while the mock request runs.
- Clear feedback for successful registration and an email address that is already registered.

After successful registration, show a confirmation with a way to return to login. Newly created accounts do not need to work in the login mock.

### 3. Forgot password

Include:

- An email address field.
- A button to request a password-reset link.
- A link back to login.
- Validation for a required, correctly formatted email address.
- A loading state while the mock request runs.
- A confirmation such as: “If an account exists for this email address, you will receive a password-reset link.”

Use the same confirmation for all valid email addresses. Sending an email and building a reset-password page are outside the scope.

## Design and usability requirements

- Create a consistent visual style across all three pages, including typography, spacing, colors, buttons, and form controls.
- Make the pages usable on mobile and desktop, with no horizontal scrolling at typical screen widths.
- Provide clear navigation between the pages.
- Use visible field labels, readable text, and sufficient color contrast.
- Make all controls usable with a keyboard and provide visible focus states.
- Associate validation messages with their fields. Do not communicate errors through color alone.
- Preserve entered values when a request fails and prevent duplicate submissions while a request is loading.

## Mock backend requirements

Keep mock request logic separate from the page components. A small service module or equivalent is sufficient.

- Simulate a short asynchronous delay so loading states can be reviewed.
- Provide a documented demo account for successful login. Other credentials should return an incorrect-credentials error.
- Provide a documented email address that triggers the already-registered sign-up error. Other valid submissions should succeed.
- Accept any correctly formatted email address in the forgot-password mock and return the generic confirmation described above.

Mock data may reset when the application reloads. A database, real email delivery, authentication tokens, and persistent sessions are not required.

## Submission

Submit a repository link or a ZIP containing the source code and a README. A hosted demo is optional.

You may use your own GitHub account and repository to complete the assessment. If you submit a GitHub repository, it must be accessible to the assessor: either make it public or invite the assessor as a collaborator with access to view and clone the repository. Confirm that access has been granted before submitting, and keep the repository accessible throughout the assessment review.

Your README should include:

- Prerequisites and exact commands to install dependencies and run the application.
- The stack and key libraries used.
- Demo credentials and instructions for exercising each mock success and error state.
- A brief explanation of your design and implementation choices.
- Approximate time spent, known limitations, and what you would improve with more time.
- Any external resources or AI tools used, and how you reviewed their output. Their use is allowed; you should be able to explain your submission.

Before submitting, check all three flows at mobile and desktop sizes and navigate the forms using only a keyboard. Include a short verification summary in the README. Automated tests are welcome but not required for this time-boxed task.

## Evaluation criteria

| Area | Weight | What we will review |
| --- | --- | --- |
| Visual design | 25% | Clear hierarchy, consistent styling, thoughtful spacing, and a polished presentation. |
| Functionality and user experience | 30% | Complete requested flows, validation, navigation, loading states, and useful feedback. |
| Code quality | 25% | Readable code, sensible component boundaries, clear state management, and separation of mock request logic. |
| Responsiveness and accessibility | 15% | Mobile and desktop usability, keyboard operation, labels, focus states, and accessible feedback. |
| Documentation | 5% | Reproducible setup, clear mock scenarios, and an honest account of decisions and limitations. |

We will assess the requested scope and the quality of your decisions within the time limit. If you run out of time, explain your priorities and tradeoffs rather than adding unfinished features.
