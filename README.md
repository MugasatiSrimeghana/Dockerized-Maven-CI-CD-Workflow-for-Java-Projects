# Dockerized Maven-CI-CD Workflow for Java Projects
This project provides a streamlined CI/CD pipeline for Java applications. By combining Maven with Docker and Jenkins, the workflow automates building, testing, packaging, and deploying applications — ensuring faster delivery and consistent quality.


## Key-Highlights
- **Automated Build**: Compile Java code with Maven, generate a JAR file, build a Docker image, and store successful artifacts..

- **Quality Assurance**: Run automated tests to validate functionality, with test reports stored for debugging and QA tracking.

- **Containerized Delivery**: Push Docker images to a container registry for easy access and deployment.

- **Continuous Integration**: Use GitHub webhooks to trigger the pipeline whenever code changes are pushed.
  
- **One-Click Deployment**: Deliver applications directly to the target environment without manual effort.

## Workflow Stages 

### This project consists of the following Stages:
### 1. Build
- **Purpose**: The ```Build``` phase handles compiling the Java source code with Maven, generating a JAR file, and creating a Docker image for the application. It also saves the produced artifacts for later reference.
- **Benefits**: Ensures the code is consistently packaged and always available in a deployable Docker image.

### 2. Test
- **Purpose**: The ```Test``` phase runs automated checks to validate functionality and quality. Test outputs are stored for review and troubleshooting.
- **Outcome**: Confirms the application is reliable, bug-free, and aligned with quality standards.

### 3. Push
- **Purpose**: The ```Push``` phase publishes the built Docker image to a container registry such as Docker Hub, making it accessible for others.
- **Benefits**: Enables easy sharing and distribution of the application in container form.

### 4. Deploy
- **Purpose**: The ```Deploy``` phase delivers the Dockerized Java application to the designated environment, making it available to users.
- **Outcome**: Provides a smooth, repeatable, and efficient deployment with minimal manual steps.

## Diagram 

<img width="1024" height="585" alt="prprprpr" src="https://github.com/user-attachments/assets/5fec4bf4-c08f-48a0-84dc-51d3909a50cc" />

## Requirements 
Before setting up the workflow, ensure you have:

- A Linux server (Ubuntu recommended) with Jenkins installed.

- A Docker Hub account (for pushing built images).

- Basic knowledge of Jenkins pipeline configuration.

## Step by step guide
| Step No | Document Link |
| ------ | ------ |
| 1 | [Configuring Jenkins and Docker][Step-1] |
| 2 | [Build Phase][Step-2] |
| 3 | [Test Phase][Step-3] |
| 4 | [Push Phase][Step-4] |
| 5 | [Deploy Phase][Step-5] |
| 6 | [Complete Phase][Step-6] |
| 7 | [Configuring Webhook][Step-7] |

   [Step-1]: <./Steps/configure.md>
   [Step-2]: <./Steps/build.md>   
   [Step-3]: <./Steps/test.md>
   [Step-4]: <./Steps/push.md>
   [Step-5]: <./Steps/deploy.md>  
   [Step-6]: <./Steps/complete.md>
   [Step-7]: <./Steps/webhook.md>


## Usage 
To get started with the CI/CD pipeline for our Java application, follow these steps:

1. **Clone this Repository**: Clone this repository to your local development environment.

   ```bash
   git clone https://github.com/MugasatiSrimeghana/Dockerized-Maven-CI-CD-Workflow-for-Java-Projects.git
   ```
2. **Configuration**: Customize the pipeline configuration to match your project's specific requirements. Adjust pipeline files, scripts, and environment variables as needed.

3. **Commit Your Code**: Add your Java application's source code to this repository, making sure it's organized in accordance with your project's structure.

4. **Set Up Pipeline Triggers**: Configure GitHub webhooks to automatically trigger the pipeline with every code push, ensuring seamless integration and deployment.
