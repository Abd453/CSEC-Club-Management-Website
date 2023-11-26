# CSEC-Club-Management-Website

```markdown
# Login Page

This project is a simple login page designed for managing access to a club management system.
 It features a user-friendly interface with a background image, form inputs for email and password, and basic authentication.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [How to Use](#how-to-use)
- [Styling](#styling)
- [Authentication](#authentication)

## Overview

The login page is a crucial component of the club management system, providing a secure way for authorized users to access the system.
 It uses basic HTML, CSS, and JavaScript for functionality.

## Features

- **Background Image:**
  - The login page features a visually appealing background image to enhance the user experience.

- **User-friendly Form:**
  - The login form includes fields for email or phone and password, making it easy for users to input their credentials.

- **Authentication:**
  - Basic authentication is implemented in JavaScript. In this example, the credentials "admin@gmail.com" and "123456" are hardcoded for simplicity.

## How to Use

1. **Accessing the Page:**
    - Open the HTML file (`login.html`) in a web browser.

2. **Entering Credentials:**
    - Input the email or phone and password in the respective fields.

3. **Logging In:**
    - Click the "Login" button to authenticate.

4. **Handling Authentication:**
    - If the provided credentials match (in this example, "admin@gmail.com" and "123456"), you will be redirected to `index.html`.
    - If the credentials are incorrect, an error message will be displayed.

## Styling

The page is styled using CSS to create a visually appealing and user-friendly interface. Key styling features include:
- Responsive design for various screen sizes.
- Background image covering the entire screen.
- Rounded corners and shadow effects for the login container, input fields, and button.

## Authentication

Authentication is handled in JavaScript. The provided credentials are checked, and if they match, the user is redirected to `index.html`. Otherwise, an error message is displayed.

Feel free to customize the styles, authentication logic, and error messages based on your specific requirements.

```

You can customize this README further based on additional features or details you want to highlight in your login page.
Club managing site.
```markdown
# Club Management System

This project is a simple web application for managing a club.
 It includes pages for management, events, member areas, and a dashboard. Additionally, it provides services information categorized into beginner, intermediate, and advanced levels.

## Table of Contents
- [Overview](#overview)
- [How to Use](#how-to-use)
- [Members List](#members-list)
- [Services](#services)
- [About Us](#about-us)
- [Notes](#notes)

## Overview

The project is built using HTML, CSS, and JavaScript.
It includes a responsive design with a navigation menu, sections for services, and a footer with social media icons.

## How to Use

1. **Navigation:**
    - Use the navigation bar to switch between different pages (Management, Event, Members Area, Dashboard).
    - The "Watch more" button is a placeholder for additional content.

2. **Adding Members:**
    - Go to the "Members Area" page.
    - Fill in the "Member Name" and "Member Email" fields in the form.
    - Click the "Add Member" button to add the member to the list.

## Members List

The list of members is stored locally using `localStorage`.
When a member is added, their information is stored, and the list is dynamically updated on the "Members Area" page.

## Services

The project provides information on services offered, categorized into beginner, intermediate, and advanced levels.

## About Us

The footer contains information about the organization, including a brief description and social media links.

## Notes

- The project uses Font Awesome for icons.
- Styling is provided through an external stylesheet (`style.css`).
- The members' information is stored locally using `localStorage`.
- This is a simple demonstration project and can be expanded based on specific requirements.


```

# Club Management System

Welcome to the Club Management System! This web application provides a platform for managing club members, events, and services. 
The system offers a user-friendly interface with various features to facilitate efficient club management.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [How to Use](#how-to-use)
- [Member Management](#member-management)
- [Services](#services)
- [About Us](#about-us)

## Overview

The Club Management System is designed to streamline the administrative tasks related to club activities.
It includes a navigation menu, a member management section, information about the services offered, and details about the club.

## Features

- **Navigation Menu:**
  - Easily navigate through different sections of the system using the responsive navigation menu.

- **Member Management:**
  - Add new members to the club by providing their name and email.
  - View the list of members in the "Members List" section.

- **Services:**
  - Explore the services offered by the club for beginners, intermediate, and advanced levels.

- **About Us:**
  - Learn more about the club through the "About Us" section, which includes social media links.

## How to Use

1. **Navigation:**
    - Use the navigation menu to access different sections of the Club Management System.

2. **Adding Members:**
    - In the "Club Management Page," use the form to add new members by providing their name and email.

3. **Viewing Members:**
    - Check the "Members List" to view the list of registered members.

4. **Exploring Services:**
    - Visit the "Services We Offer" section to learn about the club's offerings for different skill levels.

5. **About Us:**
    - Explore the "About Us" section to get more information about the club and connect on social media.

## Member Management

The Club Management Page allows administrators to add new members easily.
The list of members is dynamically updated as new members are added, providing a clear overview of the club's membership.

```javascript
function addMember() {
    // Get input values
    var name = document.getElementById('memberName').value;
    var email = document.getElementById('memberEmail').value;

    // Create list item
    var listItem = document.createElement('li');
    listItem.textContent = `${name} - ${email}`;

    // Append list item to the list
    document.getElementById('list').appendChild(listItem);

    // Clear form fields
    document.getElementById('memberName').value = '';
    document.getElementById('memberEmail').value = '';
}
```

## Services

The "Services We Offer" section provides information about the club's offerings for beginners, intermediate, and advanced levels.
Members can explore these services to find the right fit for their skill level.

## About Us

The "About Us" section gives insights into the club's mission and values. 
Connect with the club on social media platforms for the latest updates and announcements.

# Members Area

Welcome to the Members Area! This web page provides a dedicated space for managing and displaying information about club members.
Users can view the list of members and easily add new members to the club.

## Table of Contents
- [Overview](#overview)
- [Styling](#styling)
- [How to Use](#how-to-use)
- [Member List](#member-list)

## Overview

The Members Area is designed to offer a clean and organized interface for handling information about club members.
It ensures a user-friendly experience and provides a foundation for easy member management.

## Styling

The styling of the Members-Area.html page is designed to be visually appealing and user-friendly. 
The container layout ensures a comfortable viewing experience, and the color scheme contributes to a pleasant atmosphere.

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f4f4f4;
}

.container {
    max-width: 800px;
    margin: 20px auto;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
}

h2, h3 {
    color: #333;
    margin-bottom: 20px;
}

#memberList {
    border-top: 1px solid #ddd;
    padding-top: 20px;
}

ul {
    list-style-type: none;
    padding: 0;
}
```

## How to Use

1. **Viewing Members:**
    - Upon entering the page, users will see a welcoming message.
  
2. **Adding Members:**
    - To add a new member, you need to use the `addMember()` function.
    - Fill in the member's name and email in the respective input fields and click the "Add Member" button.

```javascript
function addMember() {
    // Get input values
    var name = document.getElementById('memberName').value;
    var email = document.getElementById('memberEmail').value;

    // Create list item
    var listItem = document.createElement('li');
    listItem.textContent = `${name} - ${email}`;

    // Append list item to the list
    document.getElementById('list').appendChild(listItem);

    // Clear form fields
    document.getElementById('memberName').value = '';
    document.getElementById('memberEmail').value = '';
}
```

## Member List

The "Member List" section dynamically updates as new members are added. 
Each member is displayed in a clear and concise format for easy reference.

# Dashboard Readme

## Overview

Welcome to the Dashboard of the Design Club Management System! 
This page serves as a central hub for accessing various features and information related to club management.
Users can navigate through different sections and perform actions as needed.

## Styling

The Dashboard is styled for a visually appealing and user-friendly experience. 
The layout ensures clarity and ease of use. The color scheme and fonts are chosen to provide a cohesive and pleasant design.

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f4f4f4;
}

/* Add any specific styling for the Dashboard as needed */
```

## Navigation

- **Menu:**
  - The navigation menu is accessible through the top bar, providing links to different sections of the application.
  - Users can easily switch between Management, Event, Members Area, and the Dashboard.

- **Buttons:**
  - The "Watch more" button encourages users to explore additional content.
  - The "Subscribe" button redirects users to the Management page for subscription.

# Event Page Readme

## Overview

Welcome to the Event Management section of the Design Club Management System! 
This page allows users to handle events associated with the club. 
From viewing event details to managing participant information, the Event Management page provides a comprehensive set of features.

## Styling

The Event Management page is styled to maintain consistency with the overall design of the application. It ensures a coherent and engaging visual experience.

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f4f4f4;
}

/* Add any specific styling for the Event Management page as needed */
```

## Event Services

- **Event Details:**
  - Users can find information about different levels of events, categorized as Beginner, Intermediate, and Advanced.
  - Descriptions provide details about each event category.

- **Java Script Toggle Menu:**
  - The toggle menu feature enhances user experience by providing a responsive navigation interface.

## Footer

- **About Us:**
  - The footer contains information about the club and its mission.
  - Social media icons and a LinkedIn link allow users to connect with the club.


