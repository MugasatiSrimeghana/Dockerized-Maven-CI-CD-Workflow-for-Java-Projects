# Dockerized Maven-CI-CD Workflow for Java Projects
This project provides a streamlined CI/CD pipeline for Java applications. By combining Maven with Docker and Jenkins, the workflow automates building, testing, packaging, and deploying applications — ensuring faster delivery and consistent quality.

## Workflow Diagram 

<img width="1024" height="585" alt="prprprpr" src="https://github.com/user-attachments/assets/5fec4bf4-c08f-48a0-84dc-51d3909a50cc" />


## Key-Highlights
- **Automated Build**: Compile Java code with Maven, generate a JAR file, build a Docker image, and store successful artifacts..

- **Quality Assurance**: Run automated tests to validate functionality, with test reports stored for debugging and QA tracking.

- **Containerized Delivery**: Push Docker images to a container registry for easy access and deployment.

- **Continuous Integration**: Use GitHub webhooks to trigger the pipeline whenever code changes are pushed.
  
- **One-Click Deployment**: Deliver applications directly to the target environment without manual effort.

## Requirements 
Before setting up the workflow, ensure you have:

- A Linux server (Ubuntu recommended) with Jenkins installed.

- A Docker Hub account (for pushing built images).

- Basic knowledge of Jenkins pipeline configuration.

## Workflow Stages 

### This project consists of the following Stages:
### 1. Build
- **Purpose**: The ```Build``` stage automates the compilation of our Java code, creating a JAR file with Maven. It builds a Docker image for our application and archives successful artifacts for reference.
- **Benefits**: Streamline development, ensuring that our code is deployable and readily accessible in a Docker image.

### 2. Test
- **Purpose**: The ```Test``` stage is responsible for comprehensive code testing to guarantee correctness and quality. Test results are stored for review and analysis, allowing us to maintain high code quality.
- **Outcome**: Ensure that our application is free from defects and meets our quality standards.

### 3. Push
- **Purpose**: The ```Push``` stage simplifies sharing our Docker image. It uploads the Docker image to a Docker repository, making it easily accessible to our team or end-users.
- **Benefits**: Facilitate distribution and sharing of our application in Docker form.

### 4. Deploy
- **Purpose**: The ```Deploy``` stage automates the deployment of our Java application to a designated machine, ensuring accessibility for end-users.
- **Outcome**: Achieve a reliable and efficient deployment process with minimal manual intervention.

## Steps 📝
| Step No | Document Link |
| ------ | ------ |
| 1 | [Configuring Jenkins and Docker][Step-1] |
| 2 | [Build Stage][Step-2] |
| 3 | [Test stage][Step-3] |
| 4 | [Push Stage][Step-4] |
| 5 | [Deploy Stage][Step-5] |
| 6 | [Complete Pipeline][Step-6] |
| 7 | [Configuring Webhook][Step-7] |

   [Step-1]: <./Steps/configure.d>
   [Step-2]: <./Steps/build.md>   
   [Step-3]: <./Steps/test.md>
   [Step-4]: <./Steps/push.md>
   [Step-5]: <./Steps/deploy.md>  
   [Step-6]: <./Steps/complete.md>
   [Step-7]: <./Steps/webhook.md>


## Usage 🚀
To get started with the CI/CD pipeline for our Java application, follow these steps:

1. **Clone this Repository**: Clone this repository to your local development environment.

   ```bash
   git clone https://github.com/MugasatiSrimeghana/Dockerized-Maven-CI-CD-Workflow-for-Java-Projects.git
   ```
2. **Configuration**: Customize the pipeline configuration to match your project's specific requirements. Adjust pipeline files, scripts, and environment variables as needed.

3. **Commit Your Code**: Add your Java application's source code to this repository, making sure it's organized in accordance with your project's structure.

4. **Set Up Pipeline Triggers**: Configure GitHub webhooks to automatically trigger the pipeline with every code push, ensuring seamless integration and deployment.
