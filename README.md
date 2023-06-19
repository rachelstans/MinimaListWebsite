# MinimaList
Startup website for CS260

## Description Deliverable

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

- **HTML pages** - Four HTML pages that represent the ability to select between logging in or creating an account, login, create an account, and view weekly to-do list.
- **Links** - From the home page selecting either the "Login" or "Create an account" buttons link to the correct html page. The "Github link" on the home page links to this github repo. The login page and account creation page automatically links to the weekly to-do list page.
- **Text** - Each of the to-do items is represented by a textual description.
- **Images** - On the home page there is an image of a hanging lightbulb
- **Login** - Input boxes and submit button for login and account creation.
- **Database** - The to-do list items represent data pulled from the database.
- **WebSocket** - The share icon represents the ability to share your to-do list with another user.

## CSS deliverable

For this deliverable I properly styled the application into its final appearance.

- **Header, footer, and main content body**
- **Navigation elements** - I dropped the underlines and changed the color for links.
- **Responsive to window resizing** - My app looks great on all window sizes and devices
- **Application elements** - Used good contrast and whitespace
- **Application text content** - Used 2 consistent fonts
- **Application images** - Positioned image of lightbulb to look like the dot on 'i' in Minimalist title

## JavaScript deliverable

For this deliverable I implemented by JavaScript so that the application works for a single user. I also added placeholders for future technology.

- **login/create an account** - When you press the login or create account button it takes you to the list page.
- **database** - Displayed the to-do list items. Currently this is stored and retrieved from local storage, but it will be replaced with the database data later.
- **WebSocket** - I used the setInterval function to periodically increase a random vote count. This will be replaced with WebSocket messages later.
- **application logic** - The highlight and ranking number change based up the user's selections.

## Service deliverable

For this deliverable I added backend endpoints that receives votes and returns the voting totals.

- **Node.js/Express HTTP service** - done!
- **Static middleware for frontend** - done!
- **Calls to third party endpoints** - I didn't have time to implement this. 😔
- **Backend service endpoints** - Placeholders for login that stores the current user on the server. Endpoints for voting.
- **Frontend calls service endpoints** - I did this using the fetch function.

## DB deliverable

For this deliverable I stored the votes in the database.

- **MongoDB Atlas database created** - done!
- **Endpoints for data** - My stubbed out endpoints now process the data and send it to Mongo.
- **Stores data in MongoDB** - done!

## Login deliverable

For this deliverable I associate the votes with the logged in user.

- **User registration** - Creates a new account in the database.
- **existing user** - Stores the votes under the same user if the user already exists.
- **Use MongoDB to store credentials** - Stores both user and their votes.
- **Restricts functionality** - You cannot vote until you have logged in. This is restricted on the frontend only. 😔

## WebSocket deliverable

For this deliverable I used webSocket to update the votes on the frontend in realtime.

- **Backend listens for WebSocket connection** - done!
- **Frontend makes WebSocket connection** - done!
- **Data sent over WebSocket connection** - done!
- **WebSocket data displayed** - All user votes display in realtime. I'm really proud that this is working. Way cool!

## React deliverable

For this deliverable I converted the application over to use Vue. I know it is supposed to use React, but the instructor said I could use Vue because I already have extensive experience with React.

- **Bundled and transpiled** - done!
- **Components** - Login, voting list, vote are all components.
- **Router** - Routing between login and voting components.
- **Hooks** - Vue uses class properties instead of `UseState` to track changes in vote state.
