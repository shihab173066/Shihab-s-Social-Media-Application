# Shihab's-Social-Media-Application
Module 25 Assignment
DJA01 - Social Media Application BRD

Table of Contents

1. Introduction

2. Objectives

3. Scope 

Core Features 

Additional Considerations

4. Functional Requirements 

User Management 

Post Management 

Layout & Navigation

5. Non-Functional Requirements

6. Technology Stack

7. Constraints & Timeline

8. Deliverables

9. Evaluation Criteria

10. Summary

1. Introduction

This assignment requires you to build a simple social media application using Django (backend) and HTML, CSS, JavaScript (frontend). The application mimics a basic version of Facebook by featuring:

A homepage displaying posts from all users.

A profile page that shows only the logged-in user’s posts along with options to edit or delete them.

A simple navbar and footer for navigation and basic site information.

2. Objectives

Demonstrate Django Competence: Utilize models, views, forms, template inheritance, and authentication.

User Interface & UX: Create a clean, intuitive interface with a consistent design. You may use Bootstrap / Tailwind / Raw CSS as you please, but not any other library or framework.

Core CRUD Operations: Implement Create, Read, Update, and Delete operations for posts.

User-Specific Functionality: Separate global and user-specific views.

3. Scope

Core Features
11. User Management: 

Registration: Build a registration form using Django’s built-in user model. 

Authentication: Implement login and logout functionality. 

Password Management: (Optional Bonus) Add password change and reset options.

12. Post Management: 

Homepage (Global Feed): Display posts from all users. 

User Profile Page: Show only the logged-in user’s posts. Provide options to edit or delete posts. 

Create Post: Allow users to create new posts with text and an optional image upload.

13. User Interaction & Layout: 

Navbar & Footer: 

Simple navigation bar for links to homepage, profile, login/logout, and registration. 

Basic footer with site information.

Feedback: Use Django’s message framework for notifications (e.g., "Post created successfully").

Additional Considerations

Template Inheritance: Maintain consistent layouts across all pages.

Query Optimization: Use techniques like select_related or prefetch_related where appropriate.

Security: Protect pages using mixins like LoginRequiredMixin or decorator like login_required .

Note: Focus on the core functionalities. Extra features may be added as bonus work without compromising simplicity

4. Functional Requirements

User Management

Registration:

Create a form with fields: username , email , password , and confirm password .

Validate inputs using Django's built-in validation and model forms.

Authentication:

Implement login and logout using Django’s built-in authentication views.

Provide user feedback messages on login/logout events.

Access Control:

Restrict post creation, editing, deletion, and profile management to authenticated users only.

Post Management

Homepage (Global Feed):

Display a list of posts from all users in a feed-like format.

User Profile Page:

Show only the logged-in user’s posts. Provide Edit and Delete buttons for each post (only if the user owns the post).

Create Post:

Provide a form for creating new posts with:

Text content

Optional image upload

Update & Delete Post:

Ensure that only the owner of a post can update or delete it.

Include a confirmation step before deletion.

Layout & Navigation

Navbar: Include links to the homepage, profile page, login/logout, and registration page.

Footer: Simple footer with basic information (e.g., copyright).

Feedback:Utilize Django’s messages framework to notify users about actions (e.g., “Post updated successfully”).

5. Non-Functional Requirements

Simplicity: The application must remain straightforward to ensure ease of testing and grading.

Code Quality: Write clean, well-documented code following Django best practices.

Usability: Create an intuitive UI that offers clear and immediate feedback.

Performance: Optimize database queries using Django's query optimization techniques.

Documentation: Include a comprehensive README with setup instructions and design rationale.

6. Technology Stack

Backend: Django (Python)

Frontend: HTML, CSS, JavaScript

Database: SQLite (default for Django projects)

Version Control: Git (recommended to use GitHub for submissions)

Other: Utilize Django’s built-in user model and authentication views.

7.Constraints & Timeline

Deadline: As mentioned in Ostad Platform.

Scope: Concentrate on the core functionalities; avoid unnecessary extras that complicate testing.

Testing: Manually test all features (registration, login, post creation, editing, deletion) before submission

8.Deliverables

Source Code: Submit the complete project repository. Provide a GitHub (or equivalent) repository link containing your well-organized and commented code.

README File: Your README is a critical part of your submission. It must include:

User Credentials for Testing: Supply sample user accounts with their usernames and passwords. If you create a superuser, please use admin as both the username and password.

Setup and Installation Instructions: Offer clear, step-by-step guidance on how to install and run your application locally.

Summary of Implemented Features: Briefly describe the key features of your application.

Important: Incomplete documentation in the README may result in a failing grade.

ER Diagram: Include an Entity Relationship Diagram (ERD) as an image file in your repository. This diagram should clearly illustrate your application's database structure.

Credentials: Ensure that testing credentials are clearly provided in the README. This includes:

Sample user accounts (with usernames and passwords) for regular testing, at least two.

If applicable, a superuser account using admin for both username and password.

Demonstration (Optional): You may also include a short video walkthrough of your application to showcase its features and functionality. While optional, a demonstration will be viewed favorably.

All deliverables should be included as part of your final submission. Missing any of these (without demonstration) might lead to a 0 in your assignment result.
9. Evaluation Criteria

Functionality: Does the application meet the requirements (global feed, profile page with edit/delete, user authentication, and post creation)?

Code Quality: Is the code well-organized, readable, and following Django best practices?

User Interface: Is the design clean and intuitive with a clear navbar and footer?

Documentation: Are the setup instructions and project documentation clear and complete?

10. Summary
In this assignment, you are to build a basic social media application demonstrating your proficiency with Django and frontend web development. The application should include:

A homepage displaying posts from all users.

A profile page for the logged-in user, showing their posts with options to edit or delete.

A clean, simple navbar and footer for navigation.
