# AWS To-Do App

## Overview
This AWS-based To-Do app utilizes serverless architecture to manage tasks efficiently. The backend is powered by AWS Lambda, DynamoDB, and API Gateway, while the frontend is a simple HTML file that interacts with the backend.

## Backend (AWS Services)
- **AWS Lambda:** Python-based functions to handle CRUD operations for tasks.
- **DynamoDB:** NoSQL database to store tasks.
- **API Gateway:** Routes HTTP requests from the frontend to Lambda functions.

## Frontend
- `index.html`: A simple HTML/JavaScript file that sends requests to the API Gateway.
- Can be hosted **locally**, on **AWS S3**, or **AWS Amplify** for deployment.
- Used locally for this project as it is a simple CRUD operation based project

## How to Use
### Clone the Repository
```sh
 git clone https://github.com/Aryahi/AWS-webapp.git
 cd AWS-webapp
```

### Deploy AWS Resources
Ensure that the following AWS services are set up and configured:
- **Lambda functions** for handling API requests
- **DynamoDB** table for storing tasks
- **API Gateway** for connecting frontend and backend

### Update `index.html`
Replace `<your-api-gateway-url>` with your actual API Gateway URL in `index.html`:
```js
const API_URL = "https://your-api-gateway-url.amazonaws.com/prod/";
```

### Run the Application
- Open `index.html` in a browser to interact with the app.
- Test creating, updating, deleting, and retrieving tasks.

## Deployment Options
You can host the frontend using:
- **AWS Amplify** (Recommended for easy deployment and CI/CD)
- **Local hosting** (For testing and development purposes)

## Future Enhancements
- Authentication using AWS Cognito.
- Improved UI with a frontend framework like React or Vue.
- Add more backend functionality such as due dates and task categories.

For any issues or contributions, feel free to open a pull request on GitHub! 🚀

