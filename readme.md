# Simple Web App with Jenkins Pipeline

## Table of Contents
1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Prerequisites](#prerequisites)
4. [Local Development](#local-development)
5. [Jenkins Pipeline](#jenkins-pipeline)
6. [Setup for Jenkins](#setup-for-jenkins)
7. [Deployment](#deployment)
8. [Customization](#customization)
9. [Contributing](#contributing)
10. [License](#license)

## Introduction

This project demonstrates a basic web application using HTML, CSS, and JavaScript, integrated with a Jenkins pipeline for continuous integration and deployment. It serves as an excellent starting point for beginners learning about web development and CI/CD practices.

## Project Structure

```
simple-web-app/
├── index.html
├── styles.css
├── script.js
├── Jenkinsfile
└── README.md
```

- `index.html`: The main HTML file containing the structure of the web page
- `styles.css`: CSS file for styling the web page
- `script.js`: JavaScript file for adding interactivity to the web page
- `Jenkinsfile`: Defines the Jenkins pipeline for CI/CD
- `README.md`: This file, containing project documentation

## Prerequisites

- Git
- Web browser (for local development)
- Jenkins server (for CI/CD pipeline)
- Node.js and npm (for linting tools used in the Jenkins pipeline)

## Local Development

To run this project locally:

1. Clone the repository:
   ```
   git clone https://github.com/M-Yasir-Hassan/Simple-Web-App-with-Jenkins-Pipeline.git
   cd simple-web-app
   ```

2. Open `index.html` in your preferred web browser.

3. Make changes to the HTML, CSS, or JavaScript files as needed.

4. Refresh the browser to see your changes.

## Jenkins Pipeline

The `Jenkinsfile` in this repository defines the following stages:

1. **Checkout**: Retrieves the code from the repository
2. **Lint HTML**: Checks HTML for errors and best practices using HTMLHint
3. **Lint CSS**: Checks CSS for errors and best practices using Stylelint
4. **Lint JavaScript**: Checks JavaScript for errors and best practices using ESLint
5. **Deploy**: Placeholder for deployment steps

## Setup for Jenkins

1. Ensure Jenkins is installed on your server or local machine.

2. Install Node.js on your Jenkins server.

3. Install the necessary linting tools globally:
   ```
   npm install -g htmlhint stylelint stylelint-config-standard eslint
   ```

4. In Jenkins, create a new Pipeline job:
   - Go to "New Item" in Jenkins
   - Choose "Pipeline" as the job type
   - In the job configuration, under "Pipeline", select "Pipeline script from SCM"
   - Choose Git as the SCM
   - Enter your repository URL
   - Specify the branch to build (e.g., */master)
   - Save the job configuration

5. Run the Jenkins pipeline:
   - Go to your Jenkins job
   - Click "Build Now" to start the pipeline
   - Monitor the pipeline execution and check the console output for any errors

## Deployment

The current `Jenkinsfile` includes a placeholder Deploy stage. To implement actual deployment:

1. Determine your deployment strategy (e.g., copying files to a web server, deploying to a cloud platform)
2. Add the necessary deployment steps in the Deploy stage of the `Jenkinsfile`
3. Ensure any required credentials are securely configured in Jenkins

## Customization

Feel free to modify the HTML, CSS, and JavaScript files to expand the application. You can also customize the Jenkins pipeline to fit your specific needs, such as adding more stages for testing or security scanning.

## Contributing

Contributions to improve the project are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
5. Push to the branch (`git push origin feature/AmazingFeature`)
6. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

For any additional questions or support, please open an issue in the GitHub repository.
