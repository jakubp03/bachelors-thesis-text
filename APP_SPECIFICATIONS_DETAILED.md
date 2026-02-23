# Test Management Application - Core Specifications

## Goal

The goal of this thesis is to design and implement a **full-stack web application for test management**, inspired by the Moodle system but with an emphasis on a modern user interface and specific analytical functions. The application will be built using **React** (Frontend), **Spring Boot** (Backend), and **MySQL** (Database).

The unique feature and primary contribution of this work is its focus on **self-testing and the learning process**. The application is designed to allow students to easily create tests from their own study materials and subsequently take them repeatedly. This facilitates the consolidation of knowledge through **"active recall."** The system will provide users with detailed statistics and charts, offering an immediate overview of their progress and identifying areas that require further study.

## Core Features

### 1. Authentication and User Management

- **Registration**
- **Login/Logout**

### 2. Test Creation

- **Basic Test Info:** Title, description, categories/tags.
- **Configuration:** Optional time limits and grading scales (points, percentages).
- **Question Types:**
    - Single choice (radio buttons)
    - Multiple choice (checkboxes)
    - Text response
    - True/False
    - Matching
    - Ordering
    - Flashcard
- **Multimedia Content:** Ability to add images to questions.
- **Management Tools:** Drag & drop reordering, question duplication, and a **Question Bank** for reuse.
- **Scoring:** Individual point values for each question.
- **User-Defined Categories:** Users can create, edit, and delete their own categories to organize their study materials.
- **Multi-Categorization:** A single test can be associated with **multiple categories** (Many-to-Many relationship).

### 3. Taking Tests

- **Progress Guide:** Visual progress bar.
- **Session Persistence:** Saving drafts to continue later.
- **Timer:** Countdown with alerts.
- **Navigation:** Ability to move between questions.
- **Evaluation:** Immediate results upon submission and optional display of correct answers.

### 4. Statistics and Analytics

- **User**: Attempt history, graphical progress tracking over time, average scores, and time spent per test, Number of completions, overall average score, "most failed" questions analysis, time analysis, and individual user results.
- test participiants (users who participate in test but arent authors of the test): Attempt history
- Analytics per test and per category

### 5. Sharing and Collaboration

- **Public Links:** Sharing via URL with anyone.
- **Anonymous Mode:** Taking tests without registration (limited features, no history, optional nickname entry).

---

## User Stories

### Epic 1: Registration and Authentication

- **US-1.1:** As a new user, I want to register so I can create and save my tests.
- **US-1.2:** As a registered user, I want to log in to access my tests.

### Epic 2: Test Creation

- **US-2.1:** As a user, I want to create a new test with basic information.
- **US-2.2:** As an author, I want to add a single-choice question.
- **US-2.3:** As an author, I want to add a multiple-choice question.
- **US-2.4:** As an author, I want to add a text-based question.
- **US-2.5:** As an author, I want to add an image to a question.
- **US-2.6:** As an author, I want to reorder questions using drag & drop.

### Epic 3: Taking Tests

- **US-3.1:** As a user, I want to start a test and see the first question.
- **US-3.2:** As a participant, I want to navigate between questions.
- **US-3.3:** As a participant, I want to flag a question for later review.
- **US-3.5:** As a participant, I want to save my progress and continue later.
- **US-3.6:** As a participant, I want to submit the test and see my results.
- **US-3.7:** As a participant, I want to see the correct answers after completion.

### Epic 4: Statistics and Analytics

- **US-4.1:** As a user, I want to see my full attempt history.
- **US-4.2:** As a user, I want to see my progress visualized over time.
- **US-4.4:** As an author, I want to see an overview of all test completions.

### Epic 5: Sharing and Collaboration

- **US-5.1:** As an author, I want to share a test via a public link.
- **US-5.5:** As an anonymous user, I want to take a shared test without registering.
- **US-5.6:** As an author, I want to see a list of who has taken my test.

### Epic 6: Advanced Features

- **US-6.3:** As an author, I want to import tests from Moodle.
- **US-6.5:** As a user, I want to see a leaderboard of top performers.

---

## UI/UX Wireframe Concepts

- **Dashboard:** Test overview and management.
- **Test Editor:** Workspace for building questions.
- **Test View:** A clean, focused interface for taking tests.
- **Results Page:** Feedback with graphical elements.
- **Statistics:** Interactive charts and graphs.
- **User Profile:** Personal settings and records.