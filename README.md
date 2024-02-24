Project Documentation
University Portal Project Plan

Project Overview
The University Portal project aims to centralize information and facilitate interaction between students and professors. It will provide student logins, searchable professor profiles, university announcements, and a course list.

1. Group Formation
a. There are four (4) members in our group
b. The names of the group members 
IKROMJON SHARIPOV, ID: 220448, CS2-22
Azizbek Boboqulov, ID: 221198, CS2-22
Eshkulov Sherzod, ID: 210031, CS1-22
Olimxojayev Azizxoja, ID: 220516, CS1-22

2. Project Details

a. Project Type: Web-Based Application
There are several reasons why we chose a web-based application:

Accessibility: Users can access our university portal from any device with a web browser and internet connection, without installing software.

Centralized Management: We update or maintain everything on the server-side, eliminating the need for users to download and install updates.

Collaboration: Web technologies are inherently suited for real-time collaboration or shared data.
b. Project Idea and Purpose

Project Idea:  A University Portal web application

Purpose:

Centralized Information: Provide students and faculty with a digital hub for readily accessing important university information.

Professor Profiles: Facilitate student discovery of professors based on their research expertise or teaching areas, enhancing student-professor connections.

Student and Faculty Interaction: Potentially include features for secure communication or resource sharing within the portal, subject to the scope of your project.



3. Database Design

a. Proposed Relational Database Design

Since we're using PostgreSQL, we'll design a relational database optimized for this system. Here's the core structure:

b. Three Key Tables

1. students

id (SERIAL PRIMARY KEY)
first_name (VARCHAR(255) NOT NULL)
last_name (VARCHAR(255) NOT NULL)
university_email (VARCHAR(255) UNIQUE NOT NULL)
student_id (VARCHAR(255) UNIQUE NOT NULL)
age (INT)

2. professors

id (SERIAL PRIMARY KEY)
first_name (VARCHAR(255) NOT NULL)
last_name (VARCHAR(255) NOT NULL)
university_email (VARCHAR(255) UNIQUE NOT NULL)
office_room (VARCHAR(255))
highest_degree (VARCHAR(255))
office_hours (VARCHAR(255))

3. courses (Potential Table)

id (SERIAL PRIMARY KEY)
course_code (VARCHAR(255) UNIQUE NOT NULL)
course_name (VARCHAR(255) NOT NULL)
professor_id (INTEGER, FOREIGN KEY references professors(id))

c. Primary Keys, Foreign Keys, and Relationships

Primary Keys:  Each table has a unique identifier (id), typically a SERIAL type in PostgreSQL for auto-incrementing integers.

Foreign Keys: The professor_id in the courses table creates a relationship:

One-to-Many: One professor can teach many courses, but a course is taught by only one professor.



4. Tools and Technologies

a. List of Categories

Backend (Server-Side)

Programming Language: Node.js
Web Framework: Express.js
Database: PostgreSQL

Frontend (Client-Side)

Languages: HTML, CSS, JavaScript
CSS Framework (we may use): Bootstrap, Tailwind CSS
JavaScript Framework (we may use): React or Vue.js



Additional Tools

Version Control: Git
Collaboration: 
Code Editor/IDE: VS Code, WebStorm, or other preferred editor
Package Manager: npm
Web Server: Built into Node.js

b. Git and GitHub's Role in Your Workflow
Our GitHub repository link for our project:
https://github.com/ikromsharipov/university-database-project

Source Code Management: GitHub will be the central location to store all our project code.

Documentation: Our README.md, installation guides, and other docs live right in the repository.

Collaboration: 
Team members can work on different parts of the project using branches.
Use pull requests to propose changes and review each other's code.
GitHub's issue tracker can help us organize tasks and bugs.

Version History: GitHub maintains a complete history of changes, allowing us to roll back if needed.

5. Submission Instructions
a. UniversityPortal_ProjectPlan (done)
b. Done
c. Done

Summary
Project Summary:
A team of four Computer Science sophomores is building a University Portal web application. The portal will provide centralized information, professor profiles, announcements, and a course list.

Technology: 
The project will use Node.js, Express.js, PostgreSQL for the backend, and HTML, CSS, JavaScript for the frontend.  Potential use of CSS frameworks and JavaScript frameworks is planned. Git and GitHub will be used for collaboration.


