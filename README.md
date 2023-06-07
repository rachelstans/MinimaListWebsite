# MinimaList
Startup website for CS260

### Elevator Pitch

In a world of constant distractions and overwhelming task lists, finding focus and simplicity is crucial. Enter MinimaList, the ultimate minimalist to-do list website designed to declutter your mind and amplify your productivity. With MinimaList, we strip away the unnecessary complexities, offering you a clean and elegant interface that puts your tasks at the forefront. Say goodbye to cluttered interfaces and endless features you don't need. MinimaList provides a streamlined experience, allowing you to capture, organize, and accomplish your tasks with ease. Experience the power of simplicity as you prioritize your goals and accomplish them one by one. Embrace the tranquility of a clutter-free workflow and unlock your true potential with MinimaList. Start simplifying your tasks and maximizing your productivity today.

### Design
<img width="500" alt="1" src="https://github.com/rachelstans/ToDoListWebsite/assets/101438461/de1fe446-920b-4e97-81f5-7c3c53fe2561">
<img width="500" alt="2" src="https://github.com/rachelstans/ToDoListWebsite/assets/101438461/0db4290e-b7f5-48e4-8ad2-f34cb86c8f15">
<img width="500" alt="3" src="https://github.com/rachelstans/ToDoListWebsite/assets/101438461/ee0cc380-f2a8-43c0-b20d-9d0883b21a51">
<img width="500" alt="4" src="https://github.com/rachelstans/ToDoListWebsite/assets/101438461/c38aaaa6-7bcb-46a7-9d34-7ca376c574b5">

### Key features

- Secure login over HTTPS
- Ability for admin to create and delete to-do list items
- Display of items
- Ability to check off items
- To-do list items are persistently stored
- Ability to share to-do list with another user
  - Ability for both users to collaborate in real-time on same to-do list

### Technologies

I am going to use the required technologies in the following ways.

- **HTML** - Uses correct HTML structure for application. Four HTML pages. One for the home page, one for login, one for account creation, and one for the weekly spread.
- **CSS** - Application styling that looks good on different screen sizes, uses good whitespace, color choice and contrast. Very minimalist and simple color scheme.
- **JavaScript** - Provides login, to-do item display for a week, sharing capabilities, and backend endpoint calls.
- **Service** - Backend service with endpoints for:
  - login
  - retrieving previously stored to-do items
  - retrieving items from another user's lists when sharing is turned on and both user's agree to share lists
  - submitting new to-do list items
- **DB** - Store users and items for to-do list in database.
- **Login** - Register and login users. Credentials securely stored in database. Can't use to-do list unless authenticated.
- **WebSocket** - When to-do list is shared with another user both can add and delete items at the same time and data is shared between both users.
- **React** - Application ported to use the React web framework.

## HTML deliverable

For this deliverable I added the application structure.

- **HTML pages** - Four HTML pages that represent the ability to login, create an account, and view weekly to-do list.
- **Links** - The login page and account creation page automatically links to the weekly to-do list page.
- **Text** - Each of the to-do items is represented by a textual description.
- **Images** - I couldn't figure out how to include an image and so I didn't do this.
- **Login** - Input boxes and submit button for login and account creation.
