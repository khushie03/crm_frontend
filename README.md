# crm_frontend
# InsightSync CRM Platform

Welcome to InsightSync, your comprehensive CRM (Customer Relationship Management) platform designed to manage customer relationships effortlessly and efficiently. This README will guide you through the various components of the platform and how to get started.

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
   - [Home Page](#home-page)
   - [Sign Up](#sign-up)
   - [Login Status](#login-status)
   - [Data Insertion Success](#data-insertion-success)
   - [Image Similarity](#image-similarity)
   - [Data Analytics](#data_analytics)
   - [Login Status](#login_status)
4. [Contact](#contact)

## Introduction
InsightSync is a leading provider of CRM solutions that empower businesses to manage customer relationships efficiently. Our platform offers seamless user updates and secure data access, allowing businesses to tailor their CRM solutions to fit their unique needs and workflows. 

## Installation
To install and set up the InsightSync CRM platform, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/InsightSync.git
   cd InsightSync
   ```

2. Install the necessary dependencies:
   ```sh
   npm install
   ```

3. Start the development server:
   ```sh
   npm start
   ```

The application should now be running on `http://localhost:3000`.

## Usage

### Home Page
The home page (`index.html`) is the entry point of the InsightSync platform. It provides an overview of the platform's features and a navigation menu for easy access to different sections.

![Home Page](./screenshots/home.png)

### Sign Up
The sign-up page (`signup.html`) allows new users to register for the platform. Users must provide their name, age, date of birth, country, phone number, and password.

```html
<form action="{{ url_for('register') }}" method="POST" enctype="multipart/form-data">
    <!-- form fields -->
</form>
```

![Sign Up](./screenshots/signup.png)

### Login Status
The login status page (`login_status.html`) provides an analysis of user login details. It includes a table and a bar chart to display the login status and count.

```html
<table border="1">
    <!-- table content -->
</table>
<canvas id="loginChart" width="600" height="400"></canvas>
```

![Login Status](./screenshots/login_status.png)

### Data Insertion Success
The data insertion success page (`successful_insertion.html`) informs the user that their data has been successfully inserted into the system.

```html
<div class="container">
    <h1>Success</h1>
    <p>Your data has been successfully inserted.</p>
    <a href="/" class="btn btn-primary">Go Back</a>
</div>
```

![Data Insertion Success](./screenshots/successful_insertion.png)

### Image Similarity
The image similarity page (`image_similarity.html`) displays similar products based on the provided image. It uses a flexible layout to showcase products in a card format.

```html
<div class="product-container">
    {% for image in similar_images %}
        <div class="product-card">
            <!-- product details -->
        </div>
    {% endfor %}
</div>
```

![Image Similarity](./screenshots/image_similarity.png)

## Contact
If you have any questions or need further assistance, please contact our support team at [support@insightsync.com](mailto:support@insightsync.com).

We hope you find InsightSync to be a valuable tool in managing your customer relationships effectively. Thank you for choosing us!

---

This README provides an overview of the core functionalities and setup process for the InsightSync CRM platform. For detailed documentation, please refer to the individual HTML files and the source code in the repository.
