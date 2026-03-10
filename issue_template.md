# User Story Template

**Title:**
_As a [user role], I want [feature/goal], so that [reason]._

**Acceptance Criteria:**
1. [Criteria 1]
2. [Criteria 2]
3. [Criteria 3]

**Priority:** [High/Medium/Low]
**Story Points:** [Estimated Effort in Points]
**Notes:**
- [Additional information or edge cases]

======================================*========================================
Story 1: Account Registration
Title: As a new user, I want to register with my personal details, so that I can create an identity within the habit tracking app.

Acceptance Criteria:

The registration form includes fields for Name, Username, Age, and Country.

All fields are mandatory; the "Register" button remains disabled until all fields are populated.

Upon clicking "Register," the user receives a "Registration Successful" confirmation message.

The system validates that "Age" is a numerical value.

Priority: High
Story Points: 3
Notes:

Per security constraints, these details are for session identity only and will not be used for the authentication handshake in the login story.

Story 2: Account Login (Standard Path)
Title: As a registered user, I want to log in using the system's default credentials, so that I can access my habit tracking dashboard.

Acceptance Criteria:

The login page provides fields for "Username" and "Password."

The system grants access only when the default credentials are entered.

Upon successful login, the user is redirected to the Habit Tracking home screen.

Credentials must be cleared from the browser cache/session immediately upon logout.

Priority: High
Story Points: 5
Notes:

Crucial: User-created credentials from Story 1 will not work here. Developers must hardcode or point to the specific default credentials provided in the technical spec.

Story 3: Error Feedback on Login
Title: As a user, I want to receive a clear error message if I enter the wrong credentials, so that I understand why I cannot access my account.

Acceptance Criteria:

If the entered username or password does not match the default credentials, a message appears: "Invalid username or password. Please try again."

The error message is styled in red text to indicate a failure.

The password field is cleared automatically after an unsuccessful attempt.

Priority: Medium
Story Points: 2
Notes:

This is vital because users will instinctively try to use the credentials they created in Story 1; the error message helps guide them to check for the default login info.
