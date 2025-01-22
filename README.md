# Agile-Jira-codebase

# Jira Project Creation and Epic Setup for Whitebox Learning

## Step 1: Create a Jira Project

1. **Log in to Jira**: Open your Jira instance and log in with your credentials.

2. **Navigate to the Project Creation Page**:
   - Click on the **"Projects"** menu at the top and select **"Create project"**.
   - Alternatively, click on **"Create Project"** from the homepage if prompted.

3. **Select a Project Template**:
   - Jira provides various templates like Scrum, Kanban, Bug Tracking, and more.
   - For the "whitebox-learning" project, you can choose the **Scrum** template if you're following an agile approach, or **Kanban** if you prefer continuous flow.
   - **Template choice** depends on your team’s methodology. Scrum is useful for sprints, whereas Kanban is ideal for continuous delivery.

4. **Set the Project Name and Key**:
   - In the **Project Name** field, enter **"whitebox-learning"**.
   - **Project Key**: This is a short identifier used in issue IDs (e.g., WB for Whitebox Learning). You can leave it auto-generated, or define your own key.
   - **Example**: Project Key = WB.

5. **Choose Project Lead and Permissions**:
   - The **Project Lead** is typically the person responsible for managing the project. You can select a person from your team.
   - Set the **permissions** based on your needs (either use default permissions or create custom ones).

6. **Create the Project**:
   - Once all settings are configured, click **Create** to set up the project.

---

## Step 2: Create an Epic

Once your project is created, the next step is to add an Epic. An Epic is a large body of work that can be broken down into smaller, manageable user stories.

1. **Navigate to Your Project**:
   - From the dashboard, go to **Projects** and select **"whitebox-learning"**.

2. **Create an Epic**:
   - Go to the **Backlog** section within your project.
   - On the left-hand side, click on the **"Create Epic"** link. Alternatively, you can also click on **"Create Issue"** and then select **Epic** from the issue type dropdown.
   - **Epic Name**: Enter the name of your Epic. For example, "Whitebox Learning Website Development".
   - **Epic Summary**: Describe the large feature or goal of this Epic. For example, "Develop a comprehensive learning management system including features like a contact us page, login system, scheduling, etc."
   - Set other optional fields such as priority, due date, and assign it to the relevant person.

---

## Step 3: Create User Stories Under the Epic

User stories represent smaller pieces of functionality within the Epic. These stories can be tasks or features that need to be completed.

1. **Create User Stories for Each Feature**:
   - Go back to your **Backlog**.
   - Click on **Create Issue**, select **Story** from the dropdown.
   - **Story Title**: Enter a user-friendly title for the story. For example:
     - "Create Contact Us Page"
     - "Develop Login Page"
     - "Set up Registration Form"
     - "Create Scheduling System"
     - "Build Home Page"
     - "Recordings Page"

2. **Link Stories to Epic**:
   - After creating the story, ensure to link each one to the Epic.
   - You can do this by opening each story, selecting the **Epic Link** field, and choosing the relevant Epic (e.g., Whitebox Learning Website Development).

3. **Add Detailed Description to Each Story**:
   - For each story, add a **description** of what needs to be done. 
     - Example for "Create Contact Us Page": “Design and implement a contact form with fields for name, email, and message, along with a submit button that sends an email to support@whitebox.com.”

4. **Assign Stories and Set Due Dates**:
   - Assign each user story to the relevant team member.
   - Set **due dates** if required.

---

## Step 4: Prioritize Stories and Plan Sprint (if using Scrum)

1. **Prioritize Backlog**:
   - Drag and drop stories in the **backlog** to order them based on priority (High, Medium, Low).

2. **Start Sprint**:
   - If you're using Scrum, you can now select the stories you want to work on in the next sprint.
   - Click **Start Sprint** after selecting the tasks. This creates a time-boxed sprint to work on the stories.

3. **Assign Stories to Sprint**:
   - Ensure the stories are assigned to the sprint by selecting them in the backlog and clicking on **Assign to Sprint**.

---

## Step 5: Track Progress Using Jira Boards

1. **Track in Scrum/Kanban Board**:
   - You can use the **Scrum board** (if you're using Scrum) or the **Kanban board** (if you're using Kanban) to track the status of stories.
   - You can move stories across columns like "To Do", "In Progress", "Done" based on their status.

2. **Update Issues**:
   - As developers or team members work on the stories, update the issue status. This can be done by clicking on the issue and changing its status.

---

## Step 6: Types of Stories

Here’s a list of common types of user stories you might create:

1. **Functional Stories**: Focus on specific features or functionality of the product (e.g., "As a user, I want to be able to log in so I can access my account").
   
2. **Non-Functional Stories**: Related to performance, security, or other technical concerns (e.g., "As a user, I want the website to load within 3 seconds").

3. **Technical Stories**: Focus on the architecture or technical work required to support the functionality (e.g., "Set up the database schema for user accounts").

4. **Defect Stories**: Bugs or issues that need to be fixed (e.g., "Fix issue where login button doesn't work").

5. **Spike Stories**: Research or exploration tasks that involve gathering information or experimenting with new technologies (e.g., "Investigate third-party plugins for contact form").

---

## Step 7: Managing Epics and Stories

1. **Track Epic Progress**:
   - As stories are completed, track the progress of the Epic by checking the Epic’s progress in the backlog.
   - You can use the **Epic Burndown Chart** (available in Scrum) to visualize how many stories are completed over time.

2. **Close Epic**:
   - Once all stories within the Epic are completed, you can close the Epic by updating its status to **"Done"**.

---

## Step 8: Review and Adjust

- **Review Sprint/Backlog** regularly.
- Adjust priorities or add new user stories as needed.
- Hold sprint review and retrospectives if using Scrum to ensure continuous improvement.



---

## Final Steps

1. **Monitor**: Track progress using the board and reports (Burndown Chart, Sprint Reports).
2. **Iterate**: After a sprint is completed, evaluate the performance, adjust for the next sprint, and repeat the process.