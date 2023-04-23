---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: About
layout: home
---
# Improving the nolimitGPT Web App: A Comprehensive Guide for Successors
![Alt text](/nolimitGPT-blog/nolimitgpt.png "Screenshot of nolimitGPT")

[App hosted on HerokuApp](https://rocky-falls-15188.herokuapp.com/)   
[Github source code](https://github.com/cflynn36/nolimitGPT)
## Introduction
Hey there, I'm a first-year computer science student and I'm really excited to tell you about my experience working on the nolimitGPT web app. In this blog post, I'll try my best to explain what the project is all about, what we're hoping to achieve, and how you can help make it even better!

## 1. High-Level Goal and Value of the Project
The primary aim of the nolimitGPT web app is to provide a simple and accessible SAAS web app template for anybody to use. By incorporating a user-friendly guide to advanced technologies such as OpenAI, MongoDB and Stripe, the app aims to make SAAS web app development less daunting. Through the guide, users can learn and create their own AI based webapps. Our objective is to make this technology more readily available and easy to use, saving time for people while also providing a useful resource for users interested in AI webapp  creation.

## 2. Completed Work
To date, we have achieved the following milestones:
- Established a fundamental web app framework utilizing Node.js, Express, and EJS.
- Integrated the OpenAI API for AI-driven text interactions and image generation.
- Incorporated Stripe for subscription management.
- Implemented Google OAuth for user authentication.
- Utilized MongoDB for user administration.
- Designed a responsive front-end with Webflow CSS and JavaScript.


## 3. Getting the Work Running
To run the project locally, follow these steps:

1. Clone the repository from GitHub.
2. Install Node.js and npm (Node Package Manager) if you haven't already.
3. Navigate to the project directory and run `npm install` to install dependencies.
4. Rename the provided `example.env` file to `.env` and replace the placeholders with your actual keys and credentials. To obtain the required API keys, follow the instructions below:
   - For the OpenAI API key, sign up for an account at [OpenAI](https://beta.openai.com/signup/) and follow their instructions to generate an API key.
   - For the Stripe secret key, create an account at [Stripe](https://dashboard.stripe.com/register) and navigate to the API section in the dashboard to get your secret key. Create three monthly subscription plans in Stripe and note their price IDs. Also, obtain your Stripe public key.
   - To obtain Google Client ID and Google Client Secret, visit [Google Developers Console](https://console.developers.google.com/) and create a new project. Enable the required Google APIs (e.g., Google+ API, Google OAuth2 API) and create an OAuth 2.0 client ID. You'll be provided with the client ID and secret.
   - For the MongoDB URI, sign up for an account at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register) and create a new cluster. Then, create a user with appropriate permissions, and you'll be able to generate the connection URI.
5. Set a secure `SESSION_SECRET` value in the `.env` file. This can be any long, random string.
6. Locate the following variables in the frontend JavaScript code, index.js and views/dashboard.ejs and replace them with your own values:
   - `stripePublicKey`: Your Stripe public key.
   - `priceTrial`: The price ID for the trial plan.
   - `pricePlan1`: The price ID for plan 1.
   - `pricePlan2`: The price ID for plan 2.
7. Start the server by running `npm start`.
8. Install the Stripe CLI by following the instructions provided in the [Stripe CLI documentation](https://stripe.com/docs/stripe-cli#install).
9. Run the following command to listen for webhook events on your local machine:
`stripe listen --forward-to http://localhost:3000/webhook`

10.  Open your web browser and go to `http://localhost:3000` to view the web app.




## 4. Code Comments and Explanations
Throughout the project, you will find comments explaining the purpose of each file and code snippet. This will help you understand the project structure and make changes with confidence. In particular, pay attention to the following files:

- `index.js`: The main server file. It sets up the Express app, routes, and middleware.
- `views/`: This folder contains the EJS templates for the front-end, including `chat.ejs` and `image-generator.ejs`.
- `public/`: This folder contains static assets such as CSS and JavaScript files.

## 5. Roadmap for Next Tasks
As a new contributor, you can start by working on the following tasks:
- Enhance the user experience by adding features like image galleries, voice input, and chat history.
- Integrate additional APIs for more diverse content generation.
- Improve the front-end design and responsiveness for various devices.
- Optimize server performance and handling of API calls.
- Implement user authentication and account management.

## 6. Testing Plan
For information on testing the application, please refer to the [testing](/testing/) page.


## Conclusion
The nolimitGPT web app is an exciting project with a lot of potentials. As a first-year computer science student, you have the opportunity to learn and contribute to its development. By following this blog post, you should have a clear understanding of the project's goals, the work completed so far, and how you can

