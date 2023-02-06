# Deliverable 1 - **Development Planning**

In the `ReadMe.md` at the root of your repository, include each team member's full name and GitHub username along with their chosen/assigned subsystem name.

## Milestones and Issues

In GitHub, create **milestones/issues** for this project deliverable with the assigned due dates. The milestones should be set up along both shared, [*Project Setup*](#project-setup), and individual, [*Implementation Plan*](#implementation-plan), responsibilities for this project. For example, the **Project Setup** milestone is one where it's issues will state what work will be distributed amongst the whole team. There should be one issues for each individual indicating their assigned part of the shared project setup. In addition to this team milestone/issues, there will be an additional milestones related to each specific scenario. *E.g.: If your scenario is "Sales", then you will have 3 extra milestones:*

### Milestones

- **Sales Implementation Development** plan - Your Implementation Plan for the first deliverable
- **Sales TRS Service methods** plan - Your transaction service method plan for the second deliverable
- **Sales Subsystem Implementation** plan - Your final subsystem implementaton for the third deliverable
  
### Issues

Issue(s) will need to be created for for each milestone in a timely manner. Your instructor will inform you when the issues for the specific milestone is required.

Your milestones are to be associated with the Issues that you generate for deliverable. All of your work in this lab is to be associated with git commits that reference your GitHub Issue(s). Your instructor will be using these to track your progress and participation in this project.


> You are expected to make **regular** and **frequent** commits while working on this project. **Begin early** to ensure that you have enough time to complete this group project!

## Project Setup

There are three stages to accomplishing the setup of your solution (two immediate and one for final delivery).

1. **Project Setup**
1. **Security Setup** (done for final deliverable)
1. **Scenario Setup**



The first two stages are to be completed by different team members. **Use GitHub issues** to delegate specific tasks for those stages among your team members; divide up the tasks as equitably as possible. Create an issue for **each** set of individual task assignment.

For the third stage, each team member must set up a class library for their selected scenario.

**Each** member **must** demonstrate their participation in the project setup by making small, meaningful commits. When performing commits of your code, be sure to reference the issue number in your commit so that your work can be easily distinguished by your instructor.

### Stage 1 - Project Setup

Using the techniques and practices demonstrated in class, set up the repository project files by generating the following items.

- [ ] **Repository Documentation**
  - Ensure the **`ReadMe.md`** file at the root of your repository has the following:
    - Team Name for the project
    - Group Logo
    - Team member names mapped to each person's chosen subsystem
- [ ] **Web Application Project**
  - *This should be the first project in the solution, so that it opens as the default startup project.*
  - Use **individual accounts** for the authentication when setting up the project
    - *Customization for the website's security will be addressed in **Stage 2**.*
  - Use a class-less styling system (such as [Holiday-CSS](https://holidaycss.js.org/)) for the look & feel
  - Home page for the site must include the following
    - Group Logo
    - Team member names with their Scenario/Subsystem
  - Subfolders for each scenario to organize the pages related to each scenario. Ensure there is a *default page* for each subfolder
  - Site layout must include working navigation to default pages for each subsystem as well as the team name.
  - Add project references to the class libraries when **Stage 3** is complete
  - Configure **services** and [**user secrets**](https://docs.microsoft.com/en-us/aspnet/core/security/app-secrets?view=aspnetcore-5.0&tabs=windows) (e.g.: *connection string* values) for each subsystem when **Stage 3** is complete
    - Document the names and purposes of the **user secrets** in the `ReadMe.md` at the root of the repository

### Stage 2 - Security Setup

Using the techniques discussed in class, customize the default authentication that was generated when the project was first set up. **This task must be inplace before the final submission of your team project**.

> ***NOTE:** Follow the [step-by-step instructions](./Addendum/ReadMe.md) for this semester's handling of security.

### Stage 3 - Subsystem Setup

Each team member must create a **class library project** for their subsystem. In that library, reverse engineer the database including only the tables relevant for your scenario. Ensure the generated Entity and DbContext classes are changed from being `public` to being **`internal`**. Once you have done this, inform the team member responsible for adding references and configuring service access for the web application project. **This needs to be well coordinated**.

----

## Implementation Plan

Create an initial issue where you document your overall implementation plan. This implementation plan for your scenario must address the following areas of concern. You can detail your thoughts on each area as comments to this initial issue.

<!-- - **UI Design Implementation**
  - Identify HTML elements for various parts of the UI
  - Identify which buttons/links trigger POST and GET requests
  - Include mock-up images of the user interface -->
- **Data Modelling**
  - Identify the distinct data models for the **command** and **query** aspects of the UI Design needs and the business processing needs of the system
- **Business Processing**
  - Identify specific method signatures that you would need to create for the Business Logic Layer (BLL), including the parameter types and return type of the methods.
  - For each BLL method, identify the tables/entities you will need to work with along with any important business processing requirements for the method.

The description of the issue should include a high-level Task-List of work that would need to be done. These task-list items can then be turned into their own issues for the [coding phase](./Deliverable-3.md) of the project. For example,

![](./Create_Issue_From_Task.png)


----

*Back to the [General Instructions](./README.md)*
