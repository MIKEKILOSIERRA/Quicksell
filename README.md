This project is an interactive Kanban board built using React JS. It integrates with the provided API to display and manage tickets, allowing users to group and sort the tickets dynamically. The application is responsive, visually appealing, and retains the user's view state even after page reload.


Overview

The Kanban board interacts with the provided API from https://api.quicksell.co/v1/internal/frontend-assignment to fetch tickets. Users can group the tickets by status, user, or priority and sort them by priority or title. The application is designed to be responsive and save the user's settings (grouping and sorting options) even after a page reload.

Features

Grouping:
Group tickets by Status, User, or Priority.
Sorting:
Sort tickets by Priority (descending) or Title (ascending).
Responsive Design:
Works seamlessly across different devices.
Persistent View State:
Saves the user's grouping and sorting choices even after reloading the page.

API
The application interacts with the following API:

Endpoint: https://api.quicksell.co/v1/internal/frontend-assignment

The API provides ticket data with various fields such as:

Status: The current status of the ticket (e.g., Todo, In Progress, Done).
User: The assigned user for the ticket.
Priority: The priority level of the ticket (0 to 4).
Priority Levels:
0 - No Priority
1 - Low
2 - Medium
3 - High
4 - Urgent

Usage

Display Tickets: On application load, click the Display button to fetch and display the tickets from the API.
Grouping: Select a grouping option from the dropdown (Status, User, or Priority) to reorganize the tickets accordingly.
Sorting: Use the sorting options (Priority, Title) to adjust how the tickets are ordered within the chosen group.
User Settings Persistence: The application will save your last selected group and sort order. Even after refreshing the page, the same view state will be applied.

Example UI Flow:

Select Grouping Option: Click the "Display" button, then choose to group the tickets by Status, User, or Priority.
Select Sorting Option: Once grouped, sort the tickets by Priority (high to low) or Title (A to Z).
View Persistence: Refresh the page, and the selected grouping and sorting settings will remain intact.
Customization
You can customize the Kanban board in the following ways:

UI Enhancements: Modify the CSS for different color schemes, fonts, and sizes to suit your project needs.
Ticket Fields: Extend or modify the ticket card component to display additional information from the API.
State Management: Use additional state management tools (e.g., Redux) for larger-scale applications.
Technologies Used
React: A JavaScript library for building user interfaces.
Axios: For making HTTP requests to the API.
LocalStorage: To save and retrieve the user's view state.
CSS/SCSS: For styling the Kanban board to match the provided screenshots.
