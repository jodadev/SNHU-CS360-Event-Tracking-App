# SNHU-CS360-Event-Tracking-App

## Event Tracking Application

### Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
The goal of this project was to develop an Android application that allows users to keep track of upcoming events. The application needed to support account creation and login, provide a way to add, view, edit, and delete events, and offer optional SMS reminders. I wanted the application to be straightforward, giving users a place to organize their events without having to navigate through unnecessary features.

### What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
The application includes a login screen, an event list screen, a screen for adding or editing events, and a notification settings screen. I used a table layout to display saved events so users could quickly see their event names, dates, and times. I also included an Edit button for each event to easily edit or delete an event. One thing I focused on was making the available actions clear. For example, the event form changes its heading depending on whether the user is creating or editing an event, and the Delete button only appears when editing an existing event. These decisions helped keep the interface simple while still providing the necessary functionality.

### How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?
I approached development by working on individual features and connecting them as the application progressed. I used Java for the application logic, XML for the interface layouts, and SQLite for storing user accounts and events.
One aspect I found particularly useful was how Android allows Java classes to reference UI elements through their IDs and assign listeners to handle user interactions. This made it easier to connect buttons and text fields to the appropriate functionality. I also separated database operations into a dedicated helper class instead of placing all the database logic directly inside the activities. These are techniques I would continue using when developing other applications.

### How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
I tested the application using Android emulators running Android 14 and Android 17. I checked account creation and login, event creation and editing, deletion, and whether saved events remained available after closing and reopening the application.
I also tested SMS permission handling with permission both granted and denied. For the SMS functionality, I used Android Logcat to confirm that the application successfully submitted the SMS send request without an immediate exception.
Testing was important because some problems were not obvious until I interacted with the application. It helped me identify issues with navigation, button behavior, and how different screens worked together. It also reinforced the value of testing each feature individually instead of waiting until the entire application was finished.

### Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?
One challenge was figuring out how to make the event list both readable and interactive. Displaying events was relatively straightforward, but I also needed users to be able to select an event and make changes without complicating the interface.
I addressed this by adding an Edit button to each event row and reusing the event form for both creating and updating events. The application passes the selected event's information to the form, which then displays the existing values. This avoided the need to create an entirely separate editing screen and made the application easier to maintain.

### In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
I believe the event management functionality was the strongest part of my application. It required several components to work together, including the interface, event listeners, navigation between activities, and SQLite database operations.
Being able to create an event, store it in the database, display it in the event list, and later update or delete it demonstrated my understanding of how the different parts of an Android application interact. It was also satisfying to see the functionality work as a complete system rather than as individual pieces of code.
