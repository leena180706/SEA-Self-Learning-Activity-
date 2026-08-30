# Self-Learning Activity: Agile, DevOps & Requirement Engineering

**Reference:** AWS – *What is DevOps?*, JIRA

---

## 1. Agile vs DevOps

Agile and DevOps are two approaches used in software development. Agile focuses on developing software in small steps and taking regular feedback. DevOps focuses on making the process of building, testing, releasing and maintaining software faster and smoother.

| Aspect | Agile | DevOps |
|---|---|---|
| **Main Focus** | Developing software in small steps | Delivering and maintaining software efficiently |
| **Goal** | Complete useful features regularly | Release software quickly and safely |
| **Work Process** | Uses sprints and regular planning | Uses automation and continuous delivery |
| **Teams** | Developers, testers and product team | Developers, testers, operations and security teams |
| **Feedback** | Taken during development and reviews | Collected continuously through testing and monitoring |
| **Common Practices** | Sprint planning, reviews and retrospectives | Automated testing, CI/CD and monitoring |
| **Tools** | JIRA, Trello, Azure Boards | Docker, Jenkins, Kubernetes, AWS |
| **Main Benefit** | Helps handle changing requirements | Reduces manual work and speeds up delivery |

### Example

Consider a **College Event Management System**.

Using Agile, the team can develop the system in different stages. In the first sprint, they can create student registration. In the next sprint, they can add event creation and registration. Later, they can add notifications based on student feedback.

DevOps can be used to automatically test new code and deploy updated versions of the application.

**In simple words:** Agile mainly helps the team decide **what to build and how to develop it step by step**, while DevOps helps the team **test, deliver and maintain the software efficiently**.

---

## 2. Case Study: JIRA vs Asana in Real Projects

### Overview

JIRA and Asana are tools used to organize and track project work. JIRA is commonly used for software development, while Asana is useful for managing tasks across different types of teams.

| Feature | JIRA | Asana |
|---|---|---|
| **Main Users** | Software development teams | Business and general project teams |
| **Work Items** | Stories, tasks, bugs and epics | Tasks and subtasks |
| **Agile Support** | Strong support for Scrum and Kanban | Basic project planning |
| **Bug Tracking** | Supports detailed bug tracking | Not mainly designed for bug tracking |
| **Task Tracking** | Detailed workflow tracking | Simple and visual task tracking |
| **Reports** | Sprint and development reports | Project progress and workload views |
| **Learning** | Requires some time to understand | Easier for beginners |
| **Best Fit** | Software and Agile projects | General projects and team activities |

### Real-Project Example

- **JIRA in a Food Delivery Application:**  
  A software team developing a food delivery application can use JIRA to manage tasks such as *restaurant registration*, *food search*, *cart management* and *online payment*. Developers can update the status of each task as it moves from **To Do → In Progress → Testing → Done**. Bugs found during testing can also be added and assigned to team members.

- **Asana in a College Fest:**  
  A student committee organizing a college fest can use Asana to manage activities such as *booking the venue*, *contacting sponsors*, *designing posters*, *arranging volunteers* and *promoting events*. Each activity can be assigned to a student with a deadline.

### Takeaway

JIRA is a better choice when the project involves software development, bugs and Agile practices. Asana is useful when the main requirement is simple task management and coordination between different teams.

---

## 3. Writing Effective User Stories and Acceptance Criteria

### User Story

A user story is a simple way of describing what a user wants from a software system. It helps the development team understand the requirement from the user's point of view.

A common format is:

> **As a** [user], **I want** [something], **so that** [reason].

### Example

For a **Movie Ticket Booking System**:

> As a customer, I want to select my preferred seat before booking a movie ticket, so that I can sit in a convenient place.

### Characteristics of a Good User Story

A good user story should be:

- **Independent** – It should be possible to work on it without unnecessary dependency.
- **Negotiable** – The details can be discussed between the team and stakeholders.
- **Useful** – It should provide some benefit to the user.
- **Estimable** – The team should be able to estimate the work.
- **Small** – It should be manageable within a development cycle.
- **Testable** – The completed feature should be easy to check.

### Acceptance Criteria

Acceptance criteria are the conditions that a feature must satisfy to be considered complete.

### Example

For the movie seat selection feature:

> **Given** the customer has selected a movie and show time,  
> **When** the customer selects an available seat,  
> **Then** the selected seat should be reserved for that booking.

Additional conditions can be:

1. Already booked seats should not be selectable.
2. Available seats should be clearly displayed.
3. The selected seat should appear in the booking summary.
4. The customer should be able to change the selected seat before payment.
5. The system should show a message if the selected seat becomes unavailable.

### Good Practices

1. Write requirements in simple and clear language.
2. Make every acceptance criterion specific and testable.
3. Include normal situations as well as possible errors.
4. Discuss requirements with developers and testers before development.
5. Divide large requirements into smaller user stories.

---

## 4. Advanced Requirement Elicitation Techniques

Requirement elicitation means collecting and understanding the requirements of users and stakeholders before developing a system.

### a) Interviews

An interview is a direct conversation with users or stakeholders to understand their needs and problems.

There can be different types of interviews:

- **Structured Interview:** The interviewer asks a fixed set of questions.
- **Unstructured Interview:** The conversation is more open and allows new questions to come up.

### Example

Suppose a college wants to create a **Library Management System**.

The analyst can interview librarians and ask questions such as:

- How are books currently issued?
- How do you keep track of returned books?
- How are overdue books identified?
- What information should be available to students?
- What reports are required by the librarian?

The answers can help the development team identify the required features.

### Advantages

- Provides detailed information.
- Allows questions to be asked directly.
- Helps understand problems faced by users.

### Limitations

- Interviews can take a lot of time.
- Different stakeholders may have different opinions.

### b) Ethnography

Ethnography is a technique where the analyst observes users while they perform their normal work.

Instead of only asking a librarian how books are issued, the analyst observes the complete process in the library.

### Example

While observing the library process, the analyst may find that:

- Students wait in a queue to issue books.
- Librarians manually check some records.
- Returned books are entered separately.
- Finding overdue books takes additional time.

These observations can reveal requirements that users may not mention during an interview.

### Advantages

- Shows the actual working process.
- Helps find problems that users may not explain.
- Provides a better understanding of user activities.

### Limitations

- Observation can take considerable time.
- People may behave differently when they know they are being observed.

### Other Requirement Elicitation Techniques

- **Prototyping:** Creating a basic model of the system and taking feedback.
- **Workshops:** Bringing different stakeholders together to discuss requirements.
- **Focus Groups:** Collecting opinions from a group of users.
- **Document Analysis:** Studying existing documents and reports to understand requirements.

---

## 5. Requirement Traceability Matrix (RTM)

A Requirement Traceability Matrix, commonly called **RTM**, is a table used to connect software requirements with their related modules and test cases.

It helps the development team make sure that all important requirements are implemented and tested.

### Purpose

RTM helps to:

- Check whether every requirement is covered.
- Connect requirements with test cases.
- Track the progress of requirements.
- Identify missing requirements or tests.
- Understand the effect of requirement changes.

### Example

Consider a **College Placement System**:

| Req ID | Requirement | Module | Test Case | Status |
|---|---|---|---|---|
| REQ-01 | Student can create a profile | Student Module | TC-01 | Passed |
| REQ-02 | Student can view available companies | Placement Module | TC-02 | Passed |
| REQ-03 | Student can apply for a job | Application Module | TC-03 | In Progress |
| REQ-04 | Admin can add company details | Admin Module | TC-04 | Not Started |

### Types of RTM

1. **Forward Traceability** – Connects a requirement to its related test case.
2. **Backward Traceability** – Connects a test case back to the requirement.
3. **Bidirectional Traceability** – Maintains the connection in both directions.

---

## 6. Tools for Requirement Management

Requirement management tools help teams collect, organize, update and track requirements throughout a software project.

| Tool | Description | Suitable For |
|---|---|---|
| **IBM DOORS** | Helps store, organize and trace detailed requirements | Large and complex projects |
| **JIRA** | Manages user stories, tasks, bugs and project work | Agile software teams |
| **Confluence** | Used to create and maintain project documentation | Teams working together on documents |
| **Polarion** | Helps manage requirements and different stages of software development | Enterprise projects |
| **Visure Requirements** | Provides requirement tracking and traceability features | Projects with detailed requirements |
| **Excel / Google Sheets** | Can be used to maintain simple requirement lists and RTMs | Small projects and student projects |

### IBM DOORS

IBM DOORS is a requirement management tool that helps teams organize requirements and maintain relationships between them. It is useful when a project has a large number of requirements that need proper tracking.

### JIRA

JIRA allows software teams to manage requirements using user stories, tasks and issues. It is especially useful in Agile projects where requirements may change during development.

### Confluence

Confluence is mainly used for documentation. Teams can use it to maintain requirement details, meeting notes and other project information.

### Key Takeaway

Different projects need different requirement management tools. Large and complex projects may require dedicated tools such as IBM DOORS, while smaller Agile software projects can manage their requirements using JIRA and documentation tools such as Confluence.

---

## Conclusion

Agile and DevOps help software teams improve the development and delivery process. JIRA and Asana help teams organize project activities and track work. User stories and acceptance criteria make requirements easier to understand. Interviews and ethnography help teams discover user needs. RTM helps connect requirements with testing, while requirement management tools help store and track requirements throughout the project.

Together, these methods and tools help teams build software that is well organized, easier to test and more useful to users.

---

## References

- AWS – *What is DevOps?* — https://aws.amazon.com/devops/what-is-devops
- Atlassian – *JIRA* — https://www.atlassian.com/software/jira
- Asana – *Project Management* — https://asana.com
- IBM – *IBM Engineering Requirements Management DOORS* — https://www.ibm.com/products/requirements-management-doors
