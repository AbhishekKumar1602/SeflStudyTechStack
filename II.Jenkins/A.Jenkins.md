# Jenkins
Jenkins is an open-source automation server written in Java that facilitates the continuous integration and continuous delivery (CI/CD) of software development projects. Its primary purpose is to automate the building, testing, and deployment processes, ensuring that software changes can be integrated and tested in a timely and consistent manner.

## Key Features and Aspects of Jenkins

1. **Extensibility:** Jenkins is highly extensible and supports a vast number of plugins. This extensibility allows users to integrate Jenkins with various tools and technologies, making it a versatile solution for different development environments.

2. **Build Automation:** Jenkins automates the process of building code from source control, ensuring that the application can be consistently and reliably compiled.

3. **Continuous Integration (CI):** Jenkins supports the practice of continuous integration, where code changes are regularly integrated into a shared repository. This helps identify and address integration issues early in the development cycle.

4. **Pipeline as Code:** Jenkins enables the creation of pipelines using a domain-specific language (DSL) or through a visual editor. This allows the definition of complex workflows, including building, testing, and deployment, as code, known as "Pipeline as Code."

5. **Wide Range of Plugins:** Jenkins has a rich ecosystem of plugins that provide integrations with version control systems, build tools, testing frameworks, deployment solutions, and more.

6. **Distributed Builds:** Jenkins allows the distribution of build and test workloads across multiple machines, promoting scalability and efficiency.

7. **Monitoring and Notifications:** Jenkins provides monitoring and reporting capabilities, allowing users to track the status of builds and receive notifications about build successes or failures.

8. **Security:** Jenkins includes features for securing access to the system, managing users, and controlling permissions. This is crucial for maintaining the integrity and privacy of the CI/CD process.

9. **Community Support:** Being an open-source project, Jenkins benefits from a large and active community. Users can find extensive documentation, forums, and resources to help troubleshoot issues and optimize their Jenkins setup.

10. **Integration with Cloud Services:** Jenkins can integrate with various cloud services and platforms, allowing users to leverage cloud resources for build and deployment processes.

## Jenkins's Role in Software Development and DevOps
Jenkins is a pivotal component in DevOps and Software Development, serving as an automation and integration hub throughout the software development lifecycle. Here are key aspects of Jenkins's role in this context:

1. **Continuous Integration and Continuous Delivery (CI/CD):**
- Jenkins automates the CI/CD pipeline, allowing developers to integrate code changes seamlessly. It facilitates continuous testing, building, and deployment, ensuring a reliable and efficient software development process.

2. **Automated Testing:**
- Jenkins supports automated testing, enabling the quick identification of issues during the development phase. This ensures that code changes meet quality standards before moving further in the pipeline.

3. **Build Automation:**
- Jenkins automates the build process, ensuring consistency in creating executable applications. It manages dependencies, compiles code, and generates deployable artifacts for various environments.

4. **Version Control Integration:**
- Jenkins integrates with version control systems, such as Git, enabling automatic triggering of builds based on code changes. This tight integration enhances collaboration and version management.

5. **Environment Provisioning:**
- Jenkins facilitates the provisioning of development, testing, and production environments. It ensures that these environments are consistent, reducing discrepancies between different stages of the development lifecycle.

6. **Job Scheduling and Orchestration:**
- Jenkins allows for the scheduling and orchestration of jobs, ensuring that tasks are executed in the correct sequence. This capability streamlines complex workflows and promotes automation efficiency.

7. **Monitoring and Reporting:**
- Jenkins provides monitoring and reporting capabilities, offering insights into build and deployment processes. Developers and operations teams can track performance metrics and quickly address issues.

8. **Extensibility with Plugins:**
- Jenkins's extensibility through a wide range of plugins enhances its functionality. It can be customized to integrate with various tools and technologies, making it adaptable to different project requirements.

9. **Collaboration and Notifications:**
- Jenkins fosters collaboration by providing notification features that alert teams about build statuses, issues, or failures. This enhances communication and allows for rapid response to potential problems.

10. **Support for Multiple Platforms:**
- Jenkins is platform-agnostic, supporting multiple operating systems and environments. This flexibility ensures that development teams can use Jenkins across diverse infrastructures.


## Architecture of Jenkins
Jenkins follows a Master-Slave Architecture, where the master node manages the overall orchestration of jobs and delegates the actual execution to one or more build agents. The extensibility provided by plugins allows users to customize Jenkins to suit their specific needs and integrate it with various tools and technologies.Its architecture is designed to be modular and extensible, allowing users to customize and extend its functionality through plugins. Here is an overview of the Jenkins Architecture:

1. **Master Node:**
- The Jenkins master is the central controller that oversees the entire build and deployment process.
- It manages the web-based user interface, allowing users to configure jobs, view build results, and access various Jenkins features.
- The master node is responsible for distributing jobs to available build agents, monitoring their progress, and collecting build artifacts.

2. **Build Agents/Slaves:**
- Build agents are worker machines responsible for executing the tasks assigned by the master node.
- Agents can be set up on the same machine as the master (on a smaller scale) or on separate machines (distributed build environment).
- Each agent has its own workspace where it stores files related to the jobs it executes.
- Jenkins can dynamically provision agents based on workload and release them once the job is completed.

3. **Job:**
- A job is a fundamental unit of work in Jenkins, representing a specific task or series of tasks to be executed.
- Jobs are created and configured through the Jenkins web interface or defined in code using Jenkins Job DSL or pipeline scripts.
- Jobs can include build steps, post-build actions, and triggers that define when and how the job should be executed.

4. **Workspace:**
- Each job has its dedicated workspace, which is a directory on the file system where the job's files, source code, and build artifacts are stored during its execution.
- Workspaces are isolated to prevent interference between different jobs and to maintain consistency during builds.

5. **Plugins:**
- Jenkins functionality is extended through plugins, which are Java archives (JAR files) that integrate with Jenkins to provide additional features.
- Plugins can add support for version control systems (e.g., Git, SVN), build tools (e.g., Maven, Gradle), and deployment platforms (e.g., Docker, Kubernetes).
- Users can install, configure, and manage plugins through the Jenkins web interface.

6. **Build Steps:**
- Jobs are composed of build steps that define the individual tasks to be executed during the build process.
- Build steps can include shell commands, script execution, or invocations of build tools.
- Jenkins provides a wide range of pre-built build steps, and additional functionality can be added through plugins.

7. **Schedulers:**
- Jenkins includes a built-in scheduler that determines when jobs should be executed.
- Jobs can be triggered manually by users or automatically based on various events, such as code commits, scheduled intervals, or successful completion of other jobs.
- The cron-like syntax is often used to define recurring build schedules.

8. **Artifact Repository:**
- Jenkins can integrate with artifact repositories to store and manage build artifacts generated during the build process.
- Artifacts are files produced by the build, such as JARs, WARs, binaries, or documentation.
- Common artifact repositories include Nexus, Artifactory, and the built-in Jenkins artifact repository.


## Jenkins Jobs
A job in Jenkins is like a specific task or set of tasks that Jenkins does automatically. It's a basic building block in the CI/CD process. A Jenkins job contains all the details needed to perform a particular job, such as building, testing, or deploying software. It's like a package that holds the instructions and settings for Jenkins to carry out a specific piece of work in the continuous integration/continuous deployment workflow.

### Types of Jobs

1. **Freestyle Project:**
- A freestyle project within Jenkins offers a conventional approach to configuring and executing build tasks. Through an intuitive graphical interface, users can define sequential build steps, post-build actions, and other settings.
- Ideal for straightforward build processes with linear task sequences, such as compiling a Java application, running tests, and archiving resulting artifacts.

2. **Pipeline:**
- Jenkins pipeline jobs utilize a specialized scripting language to define intricate workflows comprising stages and steps, providing a highly adaptable and programmable method for orchestrating complex build and deployment scenarios.
- Suited for projects with sophisticated build and deployment needs or those involving multiple sequential phases, such as building, testing, and deploying across diverse environments.

3. **Multiconfiguration Project:**
- Also known as matrix projects, multiconfiguration projects enable parallel execution of builds across various configurations, such as different operating systems or dependency versions.
- Utilized when simultaneous testing across multiple platforms or configurations is necessary, like evaluating a software product on diverse operating systems or with varying library versions.

4. **Folder:**
- Jenkins folders serve as organizational constructs for categorizing and managing jobs, facilitating better organization and navigation of related projects.
- Employed to group projects based on teams, projects, or other criteria, allowing for segregated management, e.g., distinct folders for frontend and backend projects.

5. **Multibranch Pipeline:**
- Multibranch pipelines automate the creation of a distinct pipeline for each branch in a version control system (e.g., Git), particularly useful for managing feature branches' build and deployment processes.
- Enables streamlined handling of simultaneous development on multiple feature branches, with each branch having its dedicated pipeline for building, testing, and deployment.

6. **Organization Folder:**
- Organization folders streamline project management within Jenkins by aligning with the organization's repository structure, automatically scanning repositories to generate pipelines for branches.
- Valuable in large organizations with diverse teams and repositories, where organization folders aid in managing and automating the pipeline creation process for various projects.

### Job Configuration

#### General Tab

1. **Description**
- "Description" field allows you to provide a brief description or summary of the job. This description is helpful for anyone looking at the Jenkins dashboard to quickly understand the purpose or function of the job.

2. **Discard Old Builds**
- "Discard Old Builds" feature allows you to automatically remove old builds to save disk space and manage the build history. 
    - A. **`Strategy`**: Choose the strategy for discarding old builds. Jenkins provides various options like:
        - I. **`Log Rotation`**: This is a commonly used strategy. It allows you to keep a specific number of builds and/or keep builds for a certain number of days.
    - B. **`Days to Keep Builds`**: Set the maximum number of days to keep builds. Jenkins will automatically discard builds older than the specified number of days.
    - C. **`Max # of Builds to Keep`**: Specify the maximum number of builds you want to keep. Jenkins will automatically remove older builds once this limit is reached.
    - D. **Advanced**
        - I. **`Days to Keep Artifacts`**: Specify the number of days to keep build artifacts. Artifacts older than this threshold will be removed.
        - II. **`Max # of Builds to Keep with Artifacts`**: If your builds produce artifacts, you can specify to keep all builds associated with a particular "artifact ID" to aid in long-term maintenance.

3. **GitHub Project**
- Link your Jenkins job directly to a GitHub project by providing the GitHub project URL. This integration facilitates seamless interaction between your Jenkins job and the corresponding GitHub repository, enabling actions such as triggering builds upon repository changes.

4. **This Project is Parameterized**
- Enable this option when your job requires parameters for dynamic customization. You can add various types of parameters:
- **`Add Parameter`**
    - A. **`Boolean Parameter`**: Accepts true/false inputs.
    - B. **`Choice Parameter`**: Provides a predefined set of choices.
    - C. **`Credentials Parameter`**: Allows selection of credentials.
    - D. **`File Parameter`**: Accepts files as input.
    - E. **`Multi-String Parameter`**: Accepts multiple string values.
    - F. **`Password Parameter`**: Ensures secure password input.
    - G. **`Run Parameter`**: Refers to another job's run as a parameter.
    - H. **`String Parameter`**: Accepts a single string value.

5. **Throttle Builds**
- Throttle Builds is a crucial feature for controlling the rate of build execution, preventing resource overload, and ensuring optimal resource utilization during peak times.
    - A. **`Number of Builds`**: Specify the maximum number of builds allowed within a certain time period.
    - B. **`Time Period`**: Define the duration for which the throttle limit applies.
    - C. **`Allow User Triggered Builds to Skip the Rate Limit?`**: Decide whether user-triggered builds can bypass the throttle limit.

6. **Execute Concurrent Builds If Necessary ?**
- This setting allows Jenkins to execute builds concurrently based on available resources. When enabled, if resource demand is high, the system can run multiple builds simultaneously, optimizing job execution.

7. **Advance**
    - A. **`Quit Period`**:  Introduces a delay before initiating a build.
    - B. **`Retry Count`**: Specifies the number of retry attempts for failed builds.
    - C. **`Block Build When Upstream Project is Building`**: Pauses the build if the upstream project is currently building.
    - D. **`Block Build When Downstream Project is Building`**: Prevents the build from proceeding if a downstream project is actively building.
    - E. **`Use Custom Workspace`**: Employs a custom workspace for the job.
    - F. **`Display Name`**: Allows customization of the displayed name for the job.
    - G. **`Keep the Build Logs of Dependencies`**: Retains build logs of dependent projects for reference and troubleshooting.
 

#### Source Code Management
- The "Source Code Management" (SCM) section in jenkin job configuration is where you define how Jenkins should interact with your version control system (VCS) to obtain the source code for your project. This section is crucial for setting up the linkage between Jenkins and your source code repository, enabling Jenkins to pull the latest code and initiate the build process

1. **None**: If your project does not involve version control or you prefer not to use SCM, you can choose the "None" option. This is suitable for cases where the source code is provided by other means.

2. **Git**: When selecting the Git option, you can configure Jenkins to interact with your Git repository. You'll typically need to provide the following details:
    - A. **`Repository URL`**: Specify the URL of your Git repository.
    - B. **`Credentials`**: Optionally, provide credentials if your repository is private, so requires authentication.
    - C. **`Branches to Build`**: Define which branches Jenkins should build. You can specify branches by name or use wildcards.
    - D. **`Additional Behaviors`**: Configure additional behaviors such as polling the repository for changes or clean checkouts before each build.

#### Build Tiggers 

1. **Trigger Builds Remotely (e.g., From Scripts)?**
- This option allows external scripts or systems to trigger builds in Jenkins remotely. When enabled, Jenkins generates a unique URL (token-based) that external entities can use to initiate builds programmatically.

2. **Build after Other Projects are Built?**
- Configure this option to trigger a build when specific projects have completed their builds. Details include:
    - A. **`Project to Watch`**: Specify the projects whose completion triggers this build.
    - B. **`Trigger Only if Build is Stable`**: Set whether the trigger should occur only if the watched project's build is stable.
    - C. **`Trigger Even if the Build is Unstable`**: Decide if the trigger should still occur even if the watched project's build is unstable.
    - D. **`Trigger Even if the Build Fails`**: Specify if the trigger should happen even when the watched project's build fails.
    - E. **`Always Trigger, Even if the Build is Aborted`**: Determine if the trigger should occur even if the watched project's build is aborted.

3. **Build Periodically?**
- Enable this option to schedule builds at specific time intervals. Use cron syntax to define the schedule, allowing for periodic builds based on time.

4. **GitHub Hook Trigger for GITScm polling?**
- If your source code management is Git and you want to trigger builds automatically on code changes, this option utilizes GitHub webhooks for triggering builds on GitScm polling.

5. **Poll SCM?**
- This option enables Jenkins to periodically poll the version control system for changes and trigger builds if changes are detected. Configure the polling schedule to determine how frequently Jenkins checks for updates.
    - A. **`Ignore Post-Commit Hooks?`**: Decide whether Jenkins should ignore post-commit hooks during the SCM polling process. If enabled, Jenkins relies solely on polling for changes.

#### Build Environments
- The "Build Environment" section in jenkin job configuration allows to specify settings and conditions that affect the overall environment in which your build runs. This section is crucial for ensuring a clean, consistent, and well-configured workspace for your build process.

1. **Delete Workspace before Build Starts**
- This option deletes the workspace before the build begins, ensuring a fresh start.
    - A. **`Advanced`**
        - I. **`Patterns for Files to be Deleted`**: Specify file patterns for deletion.
        - II. **`Apply Pattern also on Directories?`**:  Decide whether to apply deletion patterns to directories.
        - III. **`Check Parameter`**: Include additional checks before deletion.
        - IV. **`External Deletion Command`**: Use an external command for workspace deletion.
        - V. **`Disable Deferred Wipeout`**: Disable deferred workspace wipeout.

2. **Use Secret text(s) or File(s)?**
- This option allows secure usage of secret information within the build environment. Configure bindings for various secret types:
    - A. **`Bindings`**
        - I. **`Certificate`**: Binding for certificate-based secrets.
        - II. **`Git Username and Password`**: Bind Git credentials securely.
        - III. **`SSH User Private Key`**: Securely bind SSH private keys.
        - IV. **`Secret ZIP File`**: Bindings for secret information stored in ZIP files.
        - V. **`Secret File`**: Bind secret files securely.
        - VI. **`Secret Text`**: Bind secret text securely.
        - VII. **`Username and Password (Conjoined)`**: Bind combined username and password securely.
        - VIII. **`Username and Password (Separated)`**: Bind username and password separately for security.

3. **Add Timestamps to the Console Output**
- This option timestamps the console output during the build, providing a chronological record of build events for traceability and analysis.

4. **Inspect Build Log for Published Build Scans**
- This option involves inspecting the build log for published build scans, allowing integration with tools that analyze and publish build scan information.

5. **Terminate a Build if it's Stuck**
- This option provides mechanisms for handling builds that may become stuck, including setting timeouts and defining actions to take when a timeout occurs.
    - A. **`Timeout Strategy`**: Timeout Strategy refers to the method or approach employed to handle build processes that may become stuck or unresponsive. Options for Timeout Strategy includes:
        - I. **`Absolute`**: Set an absolute timeout duration.
        - II. **`Deadline`**: Specify a deadline for the build.
        - III. **`Elastic`**: Use an elastic timeout strategy.
        - IV. **`Lickly Stuck`**: Define conditions for identifying a build as likely stuck.
        - V. **`No Activity`**: Set a timeout based on no build activity.

    - B. **`Timeout Variable`**: A variable used to define the duration of the timeout. It provides flexibility in adjusting timeout durations dynamically based on specific conditions or requirements.
    - C. **`Timeout Actions`** Timeout Actions are predefined responses executed when a build reaches its designated timeout threshold. Options for Timeout Actions include:
        - I. **`Abort the Build`**: Abort the build if the timeout is reached.
        - II. **`Fail the Build`**: Mark the build as failed on timeout.
        - III. **`Writing the Build Description`**: Add a description to the build log when a timeout occurs.

6. **With Ant?**
- This option allows integration with Apache Ant, a build tool, within the build environment. You can specify Ant targets and other configurations relevant to your build process.

#### Build Setps 
- The "Build Steps" section in jenkin job configuration is where you define the actual tasks that need to be performed during the build process. These steps outline the sequence of actions Jenkins should take to build, test, and package your software. Each build step corresponds to a specific action or set of actions.

1. **Execute Shell**
- This build step allows the execution of shell commands on Unix-based systems. It is versatile, allowing you to define custom scripts or commands needed for your build process.

2. **Advanced**
    - A. **`Exit Code to Set Build Unstable`**: Specifies the exit code that, when encountered, will set the build status to "Unstable." This provides flexibility in defining the criteria for marking a build as unstable.
    - B. **`Environment Filters`**: Defines environment filters to be applied during the build process, allowing for customized configurations based on specific conditions.

3. **Add Build Steps**
    - A. **`Execute Windows Batch Command`**: Enables the execution of Windows batch commands. Useful for incorporating Windows-specific tasks into the build process.
    - B. **`Execute Shell`**: Similar to the "Execute Shell" step, this allows the execution of shell commands. It is specifically designed for Unix-based systems.
    - C. **`Invoke Ant`**: Invokes Apache Ant build tool, facilitating the build and management of Java projects. Useful for projects relying on Ant for compilation and deployment.
    - D. **`Invoke Gradle Script`**: Invokes the Gradle build tool for tasks such as compiling, testing, and packaging. Ideal for projects using Gradle as their build system.
    - E. **`Invoke Top-Level Maven Targets`**: Invokes Maven targets, enabling the build and management of Java projects. This step is suitable for projects using Apache Maven for project configuration and dependency management.
    - F. **`Run with Timeout`**: Allows you to set a time limit for the execution of a specific build step. If the step exceeds the defined timeout, the build is marked as failed.
    - G. **`Set Build Status to "Pending" on GitHub`**: Sets the build status to "Pending" on GitHub commits. This can be beneficial for indicating that the build is in progress and awaiting completion.

#### Post Build Actions 
- Post-Build Actions in Jenkins job configuration encompass a series of automated tasks or operations executed after the completion of a Jenkins job. These actions are carried out following the execution of build steps and other configured processes. They offer the flexibility to perform additional tasks, responding to the outcome of the build process. Below are various Post-Build Actions you can add to your Jenkins job:

1. **Add Post-Build Action**
    - A. **`Aggregate Downstream Test Result`**: This action aggregates test results from downstream projects, providing a consolidated view of test outcomes across the entire pipeline.
    - B. **`Archive the Artifacts`**: Archives artifacts generated during the build, preserving them for future reference or deployment. This is particularly useful for storing compiled binaries, reports, or other essential files.
    - C. **`Build Other Porjects`**: Triggers the execution of other specified Jenkins projects upon the successful completion of the current job. This facilitates the automation of related tasks in a larger workflow.
    - D. **`Publish JUnit Test Result Report`**: Publishes JUnit test results, allowing for comprehensive reporting and analysis of test outcomes. Useful for tracking and improving code quality.
    - E. **`Record Fingerprints of Files to Track Usage`**: Records fingerprints of files generated during the build process. This tracking mechanism aids in understanding the usage and propagation of specific files across different builds.
    - F. **`Git Publisher`**: Performs actions related to Git repositories, such as pushing changes, setting tags, or updating references. This is beneficial for integrating Jenkins with Git-based version control systems.
    - G. **`E-Mail Notificatins`**: Sends email notifications to specified recipients, notifying them of the build outcome. This is useful for keeping team members informed about the status of the build.
    - H. **`Editable Email Notifcations`**: Similar to email notifications but with additional configurability, allowing you to customize the content and recipients of the email notifications.
    - I. **`Set GitHub Commit Status(Universal)`**: Sets the build status on GitHub commits, providing visibility into the success or failure of builds directly on the GitHub repository.
    - J. **`Set Build Status on GitHub Commit (Depricated)`**: A deprecated option for setting the build status on GitHub commits. It is recommended to use the "Set GitHub Commit Status(Universal)" action instead.
    - K. **`Delete Workspace When Build is Done`**: Deletes the workspace associated with the Jenkins job upon completion. This can help free up disk space by removing temporary files and artifacts generated during the build process.


## Building Application with Freestyle Jobs

### Anatomy of a Build in Jenkins

1. **Job/Project:**
- A build in Jenkins is associated with a specific project or task, represented as a job. Jobs define tasks, including source code location, build steps, and post-build actions.

2. **Source Code Repository:**
- Jenkins integrates with version control systems (VCS) such as Git, Subversion, Mercurial. The source code repository is where the application code is stored.

3. **Build Trigger:**
- Builds can be triggered manually or automatically based on events like code commits, pull requests, or scheduled intervals. Jenkins supports various triggers, including SCM polling, webhook triggers, and cron-like schedules.

4. **Build Environment:**
- The build environment includes necessary tools, libraries, and dependencies. Jenkins allows configuring the build environment based on project requirements.

5. **Build Steps:**
- Build steps define the sequence of actions during the build process, e.g., compiling code, running tests, generating documentation. These tasks produce the final artifact.

6. **Build Artifacts:**
- Successful builds result in one or more artifacts – compiled binaries, libraries, or packages. Artifacts are used for deployment or distribution.

7. **Post-Build Actions:**
- After the build, define post-build actions. These can include archiving artifacts, triggering downstream builds, sending notifications, or deploying to a server.

8. **Build History:**
- Jenkins maintains a build history with details of each build, including status, duration, and console output. Valuable for troubleshooting and auditing.

9. **Console Output:**
- The console output provides real-time information about the build's progress, displaying logs, error messages, and other output.

10. **Plugins:**
- Jenkins supports an extensive plugin ecosystem, extending functionality by integrating with tools, version control systems, and third-party services.

11. **Pipeline (Optional):**
- Jenkins Pipeline allows defining the entire build process as code. It offers flexibility and control over complex build workflows, commonly used for continuous delivery and deployment.


### General Guide to Build an Application Using Freestyle Jobs

1. **Create a New Freestyle Job:**
- Click on "New Item" on the Jenkins dashboard.
- Enter a name for your job and select "Freestyle project," then click "OK."

2. **Configure the Job:**
- In the job configuration page, you'll find various sections to configure your build:
    - **`General`**: Set basic options like description and parameters.
    - **`Source Code Management`**: Configure your version control system settings (e.g., Git, SVN).
    - **`Build Triggers`**: Specify when the build should be triggered (e.g., periodically, on SCM changes).
    - **`Build Environment`**: Set up environment variables or specific configurations.
    - **`Build`**: Define the build steps. This is where you specify commands to compile, test, and package your application.
    - **`Post-Build Actions`**: Define actions to take after the build completes (e.g., archiving artifacts, sending notifications).

3. **Add Build Steps:**
- Under the "Build" section, click on "Add build step" to add individual build steps.
- Depending on your application, build steps could include commands to compile source code, run tests, and package the application for deployment.

4. **Save and Run the Job:**
- Once you've configured the job, save your changes.
- You can manually trigger the build by clicking "Build Now" on the job's dashboard or set up triggers to automatically start the build based on certain conditions.

5. **View Build Results:**
- After the build completes, Jenkins will display the build result on the job's dashboard.
- You can view console output, test reports, and other build artifacts to diagnose any issues.

6. **Iterate and Improve:**
- As you continue developing your application, you may need to modify your Jenkins job to accommodate changes in the build process or deployment pipeline.

**NOTE** To practice this steps use the [JenkinsBuildApplicationDemo](https://github.com/AbhishekKumar1602/JenkinsBuildApplicationDemo)


### Creating a Jenkins Job to Build a Java Application Using Maven

#### Overview:
This guide demonstrates how to set up a Jenkins job to build a Java application using Maven. We'll utilize a GitHub repository containing the Java application code.

#### Prerequisites:
- Ensure that Maven is installed on your system.
- Access to a Jenkins instance.

#### Steps:

1. **Access Jenkins Dashboard**:
   - Log in to Jenkins to access the Dashboard.

2. **Create a New Job**:
   - Click on "New Item" in the sidebar.
   - Enter a name for your job and select "Freestyle project".
   - Click "OK".

3. **Configure the Job**:
   - You'll be redirected to the job configuration page.
   - Fill in the following configurations:

        A. **General**: Set a description for the job (e.g., "Test Job").

        B. **Source Code Management**: 
        - Choose Git and provide the Repository URL: We are using [JenkinsBuildApplicationDemo](https://github.com/AbhishekKumar1602/JenkinsBuildApplicationDemo.git) Repository. 

        - Specify the branch to build. Here we are using `*/main` branch.
            
        C. **Build Triggers**: Define conditions for triggering the job (e.g., periodically, when changes are pushed). For now, we'll leave this as default.

        D. **Build Environment**: Configure environment settings such as JDK version, Maven version, etc. This can be left as default for now.

        E. **Build Steps**: Under "Build Steps" section, select "Add Build Step" and choose "Execute Shell" and paste the following commands:
            ```bash
            cd $WORKSPACE
            cd maven-samples/single-module
            mvn clean install
            ```

        F. **Post-Build Actions**:
        - Under "Post-Build Actions" section, select "Add Post Build Action" and choose "Archive the Artifacts".

        - Specify the files or directories to archive in "Files to Archive" section. Here we are specifying this path:
            ```bash
            maven-samples/single-module/target/*jar
            ```

#### Summary:
This Jenkins job is now configured to fetch the Java application code from the specified GitHub repository, build it using Maven, and archive the resulting artifacts. This automated process enhances development workflows and ensures consistent build environments.


## Jenkin Installation

**On Linux-Ubuntu**

1. **Download Jenkins GPG Key**
```
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
```

2. **Add Jenkins APT Repository Entry**
```
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \ https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
```

3. **Update Local Package Index**
```
sudo apt-get update
```

4. **Install Fontconfig and OpenJDK 17**
```
sudo apt-get install fontconfig openjdk-17-jre
```

5. **Install Jenkins**
```
sudo apt-get install jenkins
```

6. **Start Jenkins Service**
```
sudo systemctl start jenkins
```

7. **Enable Jenkins to Start on Boot**
```
sudo systemctl enable jenkins
```

8. **Check Jenkins Service Status**
```
sudo systemctl status jenkins
```

9. **Access Web Interface and Complete Jenkins Setup**
- Open your web browser and navigate to http://localhost:8080 .
- Enter the initial admin password prompt and obtain it from the Jenkins server using the specified command.
    ```
    sudo cat /var/lib/jenkins/secrets/initialAdminPassword
    ```
- Complete the Jenkins setup by following on-screen instructions, including plugin selection and administrator user creation.


### Changing Default Port

1. **Stop Jenkins**
```
sudo systemctl stop jenkins
```

2. **Edit Jenkins Configuration**
```
sudo nano /etc/default/jenkins
```

3. **Locate `HTTP_PORT=8080` and Modify the Port** 
```
HTTP_PORT=Desired_Port_Number
```

4. **Save the Changes and Exit the Text Editor**
```
Ctrl+S, Ctrl+X
```

5. **Restart Jenkins**
```
sudo systemctl start jenkins
```

6. **Verify the Change**:
```
sudo systemctl status jenkins
```