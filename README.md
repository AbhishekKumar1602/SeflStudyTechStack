# DevOps - ShelfStudyTechStack


![DevOps](https://github.com/AbhishekKumar1602/SeflStudyTechStack/blob/main/Temp/DevOps.png)

## Introduction to Devops
`DevOps` is a `Methodology` in the `Software Development` and `IT Industry`. Used as a set of practices and tools, DevOps integrates and automates the work of Software Development (Dev) and IT Operations (Ops) as a means for enhance the efficiency and effectiveness of the software development and delivery processes.

### Key Principles and Practices of DevOps Include

1. **Collaboration**: DevOps promotes a culture of collaboration and communication between development and operations teams. This ensures that both teams work together seamlessly throughout the entire software development lifecycle.

2. **Automation**: Automation is a crucial aspect of DevOps. By automating repetitive tasks such as code deployment, testing, and infrastructure provisioning, teams can accelerate the development and release processes while reducing errors and improving consistency.

3. **Continuous Integration**: Developers regularly integrate their code into a shared repository, and automated builds and tests are triggered. This helps identify and address integration issues early in the development process.

4. **Continuous Deployment**: Continuous Deployment involves automatically deploying code changes to production or staging environments after passing automated tests. This allows for faster and more frequent releases.

5. **Infrastructure as Code (IaC)**: Infrastructure as Code involves managing and provisioning infrastructure using code and automation tools. This enables consistent and reproducible infrastructure setups.

6. **Monitoring and Feedback**: DevOps emphasizes the importance of monitoring applications and infrastructure in real-time. This helps identify issues quickly and provides valuable feedback for continuous improvement.

7. **Microservices**: DevOps often aligns with the architectural approach of microservices, where applications are built as a collection of small, independent services. This modular approach makes it easier to deploy, scale, and update specific components without affecting the entire application.

8. **Security Integration**: DevOps incorporates security practices throughout the development lifecycle rather than treating it as a separate phase. This approach, known as DevSecOps, aims to build security into the development process from the start.


## DevOps Life Cycle
The DevOps life cycle is a comprehensive set of practices and principles designed to enhance collaboration, communication, and efficiency between development (Dev) and operations (Ops) teams throughout the entire software development process. This iterative and collaborative approach helps organizations deliver high-quality software products with greater speed, reliability, and consistency.
The DevOps life cycle typically comprises several key stages, each emphasizing specific practices and fostering a culture of continuous improvement. These stages include:

![DevOps Lifecycle](https://github.com/AbhishekKumar1602/SeflStudyTechStack/blob/main/Temp/DevOps%20Lifecycle.jpeg)

1. **Plan**: In this stage, teams define the project scope, requirements, and objectives. Planning also involves creating a roadmap, setting goals, and estimating resources required for development.

2. **Code**: Developers write and commit code to a version control system (VCS), which allows for tracking changes, collaboration, and versioning. Continuous integration practices may be employed at this stage to ensure that code changes integrate seamlessly.

3. **Build**: The code is compiled, integrated, and built into executable files or artifacts. This stage ensures that the software is compiled correctly and is ready for testing.

4. **Test**: The software undergoes various testing phases, including unit testing, integration testing, and system testing. Automated testing is often emphasized in DevOps to catch defects early and ensure the reliability of the software.

5. **Release**: Once testing is successful, the software is prepared for release. This involves creating a deployment package and documenting release notes. Continuous delivery practices aim to automate this process, making releases more frequent and reliable.

6. **Deploy**: The release is deployed to the target environment, whether it's a staging environment for further testing or a production environment for live usage. Automation tools and practices are commonly used to ensure consistent and reliable deployments.

7. **Operate**: After deployment, the software is actively monitored and managed in a production environment. Operations teams are responsible for ensuring the system's availability, performance, and security.

8. **Monitor**: Continuous monitoring is crucial for identifying and addressing issues proactively. Monitoring tools track system performance, user behavior, and other relevant metrics. This information is used to improve the system's overall reliability and performance.

## DevOps Pipeline
A DevOps pipeline is a set of automated processes and tools that facilitate the continuous integration, delivery, and deployment of software applications. It is a key component of the DevOps methodology, which aims to improve collaboration and communication between development and operations teams, ultimately streamlining the software development lifecycle. The DevOps pipeline typically consists of several stages, each serving a specific purpose in the software delivery process. These stages may include:

A. **Continuous Development:** Continuous Development within the DevOps framework revolves around an iterative and ongoing approach to software evolution. This practice places a strong emphasis on constant improvement through regular updates and enhancements. By integrating feedback from users and stakeholders, teams can seamlessly deliver new features, improvements, and bug fixes in response to dynamic requirements and market demands. The iterative nature of Continuous Development ensures adaptability and agility in software development processes.

B. **Continuous Integration:** Continuous Integration is a pivotal practice in DevOps that revolves around the automatic integration of code changes from various contributors into a shared repository. The primary objective is to identify and address integration issues early in the development cycle. Through automated building and testing of integrated code, Continuous Integration systems provide rapid feedback to developers. This not only upholds code quality but also reduces integration problems, ensuring that the software is consistently in a deployable state.

C. **Continuous Testing:** Continuous Testing extends beyond traditional testing phases by integrating testing activities seamlessly into the CI/CD pipeline. This involves automating the testing process throughout the development lifecycle. Automated tests are executed whenever changes are introduced to the codebase, preventing the introduction of defects or disruptions to existing functionality. Continuous Testing, by offering fast and continuous feedback on software quality, supports the rapid and reliable delivery of software.

D. **Continuous Deployment:** Continuous Deployment is the practice of automatically deploying code changes to production or a production-like environment following the completion of continuous integration, testing, and monitoring stages. The ultimate goal is to swiftly and efficiently deliver new features, enhancements, or bug fixes to end-users. This streamlining of the release process reduces manual interventions and ensures the consistent and reliable delivery of the latest code to production environments, fostering a seamless and efficient deployment pipeline within the DevOps life cycle.

E. **Continuous Monitoring:** Continuous Monitoring in the DevOps context involves the ongoing observation and measurement of system performance, availability, and other critical metrics. Utilizing monitoring tools, this practice allows real-time tracking of application behavior, infrastructure performance, and other components. Continuous Monitoring plays a vital role in promptly identifying issues, anomalies, and performance bottlenecks. By continuously collecting and analyzing data, teams can ensure the reliability and optimal performance of the software in production, contributing to a responsive and resilient system.

1. **Code Repository**:
    - The code repository is where the source code for the application is stored. It serves as a centralized location for version control, collaboration, and tracking changes.
    - Git is the most widely used version control system. Platforms like GitHub, GitLab, and Bitbucket provide hosting and collaboration features.

2. **Continuous Integration**:
    - Continuous Integration involves automatically integrating code changes from multiple contributors into a shared repository. The goal is to detect and address integration issues early in the development process.
    - Jenkins, Travis CI, GitLab CI, and CircleCI are popular CI tools. They automate the build and testing processes triggered by code changes.
    
3. **Automated Testing**:
    - Automated testing ensures that code changes don't introduce new bugs or break existing functionality. It includes unit, integration, and end-to-end testing.
    - For unit testing, tools like JUnit, NUnit, and Pytest are common. Selenium, JMeter, and Postman are used for integration and end-to-end testing.

4. **Artifact Repository**:
    - An artifact repository stores and manages the build artifacts generated during the CI process. These artifacts can include compiled code, libraries, and dependencies.
    - Artifactory and Nexus are popular artifact repository tools. They support various package formats and help in versioning and managing dependencies.

5. **Continuous Deployment**:
    - Continuous Deployment automates the deployment of applications to various environments, ensuring a consistent and repeatable process.
    - Ansible, Puppet, Chef, and Docker are often used for configuration management and containerization. Kubernetes is widely used for orchestrating containerized applications.

6. **Infrastructure as Code (IaC)**:
    - IaC involves managing and provisioning infrastructure using code, making it more scalable and repeatable. It ensures consistency between different environments.
    - Terraform, AWS CloudFormation, and Ansible are popular IaC tools. They allow defining infrastructure configurations in a declarative manner.

7. **Monitoring and Logging**:
    - Monitoring and logging provide visibility into application performance, resource utilization, and potential issues. It helps in identifying and addressing issues quickly.
    - Prometheus, Grafana, ELK Stack (Elasticsearch, Logstash, Kibana), and New Relic are commonly used for monitoring and logging

8. **Feedback Loop**:
    - The feedback loop ensures that information about application performance, user feedback, and issues is communicated back to the development and operations teams.
    - Integration with collaboration tools like Slack, Jira, and Email, along with custom dashboards from monitoring tools, helps in creating an effective feedback loop.

## ShelfStudyTechStack Contents

- [DevOps RoadMap](https://github.com/AbhishekKumar1602/SeflStudyTechStack/blob/main/Temp/Devops%20RoadMap.pdf)
- [Operating System](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/1.Operating%20System)
- [Computer Networks](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/2.Computer%20Networks)
- [Linux](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/3.Linux)
- [Python](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/A.Python)
- [Bash](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/B.Bash)
- [Data Serialization Languages](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/C.Data%20Serialisation%20Languages)
- [Git and GitHub](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/I.Git%20and%20GitHub)
- [Jenkins](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/II.Jenkins)
- [Docker](https://github.com/AbhishekKumar1602/SeflStudyTechStack/tree/main/III.Docker)