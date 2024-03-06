# Docker
Docker serves as a comprehensive platform that facilitates the seamless development, distribution, and execution of applications through the use of containers. Containers provide a standardized unit wherein developers can encapsulate an application along with its dependencies, ensuring consistent performance across diverse environments, from development and testing to deployment.

## Key Features and Aspects of Docker

1. **Portability:** Docker containers encapsulate an application and its dependencies, ensuring consistency across different environments. This makes it easy to move applications between development, testing, and production environments without compatibility issues.

2. **Isolation:** Docker containers isolate applications from the underlying system and from each other. This isolation ensures that applications run consistently, regardless of differences in the host environment.

3. **Resource Efficiency:** Containers share the host OS kernel, which makes them lightweight compared to virtual machines. Docker containers can start and stop quickly, leading to efficient utilization of system resources.

4. **Version Control:** Docker images can be versioned, allowing developers to track changes to the application and its dependencies over time. This makes it easier to roll back to a previous version if needed.

5. **Scalability:** Docker makes it easy to scale applications horizontally by running multiple containers across different hosts. Containers can be quickly deployed or scaled down based on demand.

6. **Flexibility:** Docker supports a wide range of application stacks and programming languages. It allows developers to package an application and its dependencies into a single container, regardless of the underlying technology.

7. **DevOps Integration:** Docker integrates well with DevOps tools and practices. Continuous integration and continuous deployment (CI/CD) pipelines can be easily set up with Docker, streamlining the development lifecycle.

8. **Security:** Docker provides a level of security through container isolation. Each container runs in its own user space, limiting the potential impact of security vulnerabilities. Additionally, Docker has features like namespace isolation and control groups to enhance security.

9. **Rapid Deployment:** Docker containers can be started and stopped quickly, facilitating rapid deployment of applications. This is particularly beneficial in dynamic and rapidly changing environments.

10. **Microservices Architecture:** Docker is well-suited for microservices architectures. Applications can be decomposed into smaller, independently deployable containers, making it easier to develop, test, and maintain complex systems.

11. **Ecosystem and Community:** Docker has a large and active community, which means there is a wealth of documentation, tutorials, and third-party tools available. This makes it easier for developers to find solutions to problems and stay updated on best practices.

12. **Cost Savings:** Docker's resource efficiency and scalability can lead to cost savings in terms of hardware, as more containers can be run on the same infrastructure compared to traditional virtualization. 


## Key Differences Between Docker Containers and Conventional Machine

1. **Isolation and Portability**
- **Docker:** Applications and their dependencies are packaged together in containers, providing isolation from the underlying system. This ensures that the application runs consistently across different environments, making it highly portable.
- **Conventional Machine:** Applications often rely on the system's configuration and dependencies, making them less portable. Changes in the underlying system can impact the application's behavior.

2. **Resource Efficiency**
- **Docker:** Containers share the host system's kernel and use resources more efficiently than virtual machines. They have lower overhead and can start up quickly.
- **Conventional Machine:** Running applications directly on the host system may lead to resource contention and less efficient utilization, especially in cases where applications have conflicting dependencies.

3. **Dependency Management**
- **Docker:** Containers encapsulate dependencies, libraries, and the application itself. This helps in avoiding conflicts with other applications or system-level dependencies.
- **Conventional Machine:** Applications may rely on specific versions of libraries and dependencies. Managing these dependencies can be challenging and may lead to conflicts or compatibility issues.

4. **Isolation of Processes:**
- **Docker:** Containers isolate processes, making it possible to run multiple applications with different dependencies on the same host without interference.
- **Conventional Machine:** Applications running directly on the host system may interfere with each other, especially if they have conflicting dependencies or resource requirements.

5. **Consistency Across Environments**
- **Docker:** Docker containers ensure consistency in development, testing, and production environments, reducing the "it works on my machine" problem.
- **Conventional Machine:** Variations in system configurations can lead to inconsistencies between development and production environments.

6. **Ease of Deployment and Scaling**
- **Docker:** Docker facilitates easy deployment and scaling of applications. Containerized applications can be deployed consistently across different environments and scaled horizontally.
- **Conventional Machine:** Deploying and scaling applications on conventional systems may involve more manual configuration and may be less scalable.

7. **Versioning and Rollbacks**
- **Docker:** Docker images can be versioned, allowing for easy rollbacks and updates. This enhances the ability to manage application versions effectively.
- **Conventional Machine:** Versioning and rollback processes may be more complex and manual, involving backups or other mechanisms.

> **NOTE:** Docker provides a more lightweight, portable, and efficient way to package, distribute, and run applications compared to conventional systems where applications often rely on the host environment. Docker's containerization approach offers benefits in terms of consistency, scalability, and ease of management.


## Key Differences Between Docker Containers and Virtual Machines

1. **Architecture**
- **Docker:** Docker uses containerization, which involves encapsulating an application and its dependencies into a container. Containers share the host operating system's kernel but run in isolated user spaces.
- **Virtual Machines:** VMs, on the other hand, involve running a hypervisor on the host machine, which then creates multiple virtualized operating systems, each with its own kernel. Each VM runs a complete guest operating system.

2. **Resource Overhead**
- **Docker:** Containers are lightweight and share the host OS kernel, resulting in lower resource overhead. They start up quickly and use resources more efficiently than VMs.
- **Virtual Machines:** VMs have higher resource overhead because they include a full guest OS and emulate hardware. This can lead to longer startup times and increased resource usage.

3. **Isolation**
- **Docker:** Containers provide process-level isolation. Each container runs as an isolated process on the host system, but they share the same OS kernel.
- **Virtual Machines:** VMs provide stronger isolation because they emulate an entire operating system, including its kernel. This makes VMs more secure in some contexts.

4. **Portability**
- **Docker:** Containers are highly portable. Docker containers can run consistently across different environments as long as they have the Docker runtime installed.
- **Virtual Machines:** VMs are less portable because they encapsulate an entire operating system. Moving VMs between different hypervisors or cloud platforms can be more complex.

5. **Performance**
- **Docker:** Containers generally have better performance due to their lightweight nature and reduced overhead. They share the host OS kernel, allowing for more efficient resource utilization.
- **Virtual Machines:** VMs may have higher performance overhead due to the emulation of hardware and the need for a full guest OS.

6. **Scalability**
- **Docker:** Containers are designed for horizontal scaling. It's easy to deploy and scale multiple containers on a host machine or across multiple machines.
- **Virtual Machines:** VMs are traditionally scaled vertically by adding more resources to a single VM. Horizontal scaling with VMs can be more complex.

7. **Start-Up Time**
- **Docker:** Containers start up quickly since they don't need to boot an entire operating system.
- **Virtual Machines:** VMs typically have longer startup times because they need to boot a complete OS.

8. **Use Cases**
- **Docker:** Docker is well-suited for microservices architectures, continuous integration and delivery (CI/CD), and environments where lightweight, portable, and scalable solutions are required.
- **Virtual Machines:** VMs are often used in scenarios where strong isolation or compatibility with different operating systems is necessary, such as legacy applications or when running multiple operating systems on a single host.

> **NOTE:** Docker and virtual machines (VMs) are both technologies that enable the isolation of applications, but they differ in their approach and the level of abstraction they provide. Containers are lightweight, portable, and efficient, while virtual machines provide stronger isolation and are more versatile in running different operating systems. The choice between Docker and virtual machines depends on specific use case requirements and preferences. In many modern applications and development workflows, both technologies may be used together for optimal results.

## Docker's Role in DevOps and Software Development
Docker plays a crucial role in DevOps and Software Development by providing a containerization platform that allows developers to package and distribute applications, along with their dependencies, in a consistent and reproducible manner. Here are some key aspects of Docker's role in DevOps and Software Development:

1. **Isolation and Portability:**
- Docker containers encapsulate an application and its dependencies, ensuring isolation from the underlying infrastructure. This isolation makes it easier to maintain consistency across different environments, such as development, testing, and production.
- Containers are portable, meaning they can run consistently across various environments, reducing the "it works on my machine" problem. This portability simplifies the deployment process and improves collaboration between development and operations teams.

2. **Consistency and Reproducibility:**
- Docker provides a consistent environment for developers, eliminating the "it works on my machine" issue. This consistency ensures that applications run the same way in different environments, reducing the likelihood of errors caused by differences in system configurations.

3. **Efficient Resource Utilization:**
- Docker containers share the host operating system's kernel, which makes them lightweight compared to traditional virtual machines. This results in efficient resource utilization and faster startup times.
- The lightweight nature of containers allows for higher density on a single host, enabling more efficient use of resources in both development and production environments.

4. **Microservices Architecture:**
- Docker facilitates the adoption of microservices architecture by enabling the deployment of individual components as separate containers. Each microservice can be developed, tested, and deployed independently, promoting agility and scalability.

5. **Continuous Integration and Continuous Deployment (CI/CD):**
- Docker containers integrate seamlessly with CI/CD pipelines. Developers can build, test, and deploy applications in a consistent environment throughout the development lifecycle.
- CI/CD tools can use Docker images to create reproducible build environments, ensuring that the same set of dependencies is used in both development and production stages.

6. **Versioning and Rollback:**
- Docker images are versioned, allowing developers to roll back to previous versions easily in case of issues. This versioning helps in maintaining a history of changes and provides a mechanism for reliable and predictable deployments.

7. **Scalability:**
- Docker containers are designed to scale horizontally, making it easier to handle increased workloads by adding more containers. This scalability is crucial for applications with varying resource demands.

8. **Infrastructure as Code (IaC):**
- Docker configurations can be managed as code, allowing for the automation of infrastructure setup and deployments. This aligns with the principles of Infrastructure as Code (IaC) and helps in maintaining consistency and repeatability.

## Architecture of Docker
Docker follows Client-Server Architecture, which includes the three main components that are Docker Client, Docker Host, and Docker Registry. This architecture facilitates a modular and scalable approach to containerized applications, making it easy to develop, deploy, and manage applications across different environments. Here is an overview of the Docker Architecture:

1. **Docker Client:**
- The Docker Client is the user interface to Docker. It accepts commands from the user and communicates them to the Docker daemon. Users can interact with Docker through the command line interface (CLI) by typing commands like docker run, docker build, etc.
- The Docker Client can run on the same machine where Docker is installed or connect to a remote Docker daemon, allowing users to manage containers on different hosts.
- It communicates with the Docker daemon using the Docker Remote API, typically over a Unix socket or a network interface.

2. **Docker Host (Docker Daemon):**
- The Docker Host, often referred to as the Docker daemon or engine, is a background process responsible for managing Docker containers on a given machine.
- It listens for Docker API requests and handles tasks such as building, running, and stopping containers. It also manages the lifecycle of containers, ensuring they have the necessary resources and isolating them from each other.
- The Docker daemon communicates with the operating system's kernel to create and manage containers. It can run as a system service on the host machine.

3. **Docker Registry:**
- Docker Registry is a storage system for Docker images. Images are snapshots of a file system with the necessary application code, libraries, and dependencies to run a container.
- Docker Hub is a public registry where users can share and access images, but organizations often set up private registries for security and control. This allows them to store proprietary images and control access to them.
- Docker images are pulled from a registry to the local machine when a user wants to run a container. Images can be versioned, allowing for consistency and reproducibility in deploying applications.
- There are two types of registries in Docker, Public Registries, commonly known as Docker Hub, and Private Registries. Public Registries are widely accessible and used for sharing images publicly, while Private Registries are employed within enterprises for sharing images internally.


## Docker Objects
Docker objects" refer to the fundamental entities or components that Docker uses to manage and deploy containerized applications. These objects are essential building blocks that contribute to the functionality and structure of Docker-based systems. The key Docker objects include:

1. **Docker Image:**
- An image is a lightweight, standalone, and executable package that includes everything needed to run a piece of software, such as code, runtime, libraries, environment variables, and config files.
- Images are often created from a set of instructions in a Dockerfile, specifying the base image, software dependencies, and setup steps.
- Images are immutable, meaning they do not change once created. Any modifications result in the creation of a new image version.
- Images are stored in a registry (e.g., Docker Hub) and can be pulled to run on any system supporting Docker.

2. **Docker Container:**
- A container is a running instance of a Docker image, providing an isolated execution environment for the application and its dependencies.
- Containers share the host OS kernel but have their own filesystem, processes, and network, ensuring isolation from the host and other containers.
- Containers are dynamic and can be started, stopped, moved, and deleted. They encapsulate an application and its runtime environment.
- Containers are ephemeral, with changes made during runtime discarded when the container is stopped unless explicitly committed to a new image.

> **NOTE:** An image is a static, immutable blueprint for software, while a container is a dynamic, runnable instance of that image. Images serve as packaging for software distribution, while containers provide an isolated and consistent runtime environment for applications.

3. **Docker Networking:**
- Docker Networking enables communication between Docker containers and other networked entities. It allows containers to connect with each other or with external networks, facilitating the creation of complex, interconnected applications.
- Docker provides various network drivers that offer different features and performance characteristics, allowing users to choose the most suitable networking solution based on their application requirements. Docker contains the following network drivers:
     - **`Bridge`** - Bridge is a default network driver for the container. It is used when multiple docker communicates with the same docker host.
     - **`Host`** - It is used when we don't need for network isolation between the container and the host.
     - **`None`** - It disables all the networking.
     - **`Overlay`** - Overlay offers Swarm services to communicate with each other. It enables containers to run on different docker hosts.
     - **`Macvlan`** - Macvlan is used when we want to assign MAC addresses to the containers.

4. **Docker Storage:**
- Docker Storage manages the data persistence and storage aspects of containers. It allows containers to read and write data, ensuring that data persists beyond the container's lifespan.
- Storage drivers in Docker enable the interaction between containers and the underlying storage infrastructure, allowing for flexibility and compatibility with various storage solutions.
- Docker offers the following options for the Storage:
     - **`Data Volume`**: Data Volume provides the ability to create persistence storage. It also allows us to name volumes, list volumes, and containers associated with the volumes.
     - **`Directory Mounts`**: It is one of the best options for docker storage. It mounts a host's directory into a container.
     - **`Storage Plugins`**: It provides the ability to connect to external storage platforms.

5. **Docker Services:**
- Docker Services define the desired state of a group of containers, allowing for the deployment and scaling of applications across a cluster of Docker nodes.
- Services make it easier to manage and scale multi-container applications. They define how many replicas of a containerized application should run, ensuring high availability and load balancing.
- Docker Swarm, a native clustering and orchestration tool, is often used in conjunction with Docker Services to deploy and manage applications at scale. Services can be updated and rolled back, and they provide features for distributing and balancing containers.


## Basic Dockers Commands

**List All Images Present Locally**
```
docker images
```

**Pull Images From Docker Hub**
```
docker pull image_name:version
```

**Create Containr From Existing Image**

```
docker run image_name
```
- NOTE: It will create a container or pull the image of latest version if not present locally and then create container. 
 
```
docker run  image_name:version
```
- NOTE: It will create a container of specified version or pull the image of specified version if not present locally and then create container. 

```
docker run -d image_name
```
- NOTE: `-d` flag stands for "detached" mode. It will create and run the container in the background, allowing us to continue using the terminal for other commands.

```
docker run -it image_name
```
- NOTE: `-it` flag stads for "interactive terminal". It will create and run the container and will open the interactive terminal of that container.

```
docker run --name CustomContainerName image_name
```
- NOTE: `--name` flag  allow to specify a custom name for the container.

```
docker run -itd --name CustomContainerName image_name
```

**List All Runing Containers**
```
docker ps
```
- NOTE: It will list only running containers.
```
docker ps -a
```
- NOTE: It will list all running and stoped containers.

**Stop Running Container**
```
docker stop <container_name/id>
```

**Restart Stoped Container**
```
docker start <container_name/id>
```

**Opening Interactive Terminal of a Running Container**
```
docker exec -it <container_name/id> /bib/bash
```

##  Host Port and Container Port

**Host Port:**
- The host port is the port on the host machine that is mapped to the container port.
- It is the port through which you can access the services running inside the Docker container from the host machine or external systems.
When you use the -p option with Docker to map ports, you are specifying the host port.

**Container Port:** 
- The container port is the port on which a service inside the Docker container is running.
- It is the port to which applications inside the container bind to receive incoming network traffic.
- When you expose a port in a Dockerfile or with the -p option when running a container, you are specifying the container port.

**Example** 
```
docker run -p 6000:80 nginx
```
- 6000 is the host port, meaning you can access the services from the host machine on port 6000.
- 80 is the container port, indicating the service inside the container is listening on port 80.
- In this scenario, if we point our web browser to http://localhost:6000, we are accessing the NGINX web server running inside the Docker Container on its port 80.

## Docker Networking
Docker provides a versatile networking system to facilitate communication between containers and external services. Containers must be connected to a Docker network to establish network connectivity, and the available communication routes depend on the network connections.

### Docker Built-In Network Drivers:

1. **Bridge:**
- Establishes a virtual bridge between the host and containers for internal communication.
- Functionality:
      - Enables containers to communicate within the network using IP addresses and DNS names.
      - Isolates containers from external networks while allowing them to share the host's network for internet and LAN access.
      - Suitable for diverse scenarios, facilitating seamless communication between containers and providing access to the host's network.

2. **Host:**
- Integrates containers with the host's network stack without isolation.
- Functionality:
      - Containers use the host's network, eliminating the need for separate IP addresses.
      - Port binds are directly published to the host's network interface.
      - Ideal for situations requiring direct port binding to the host's interfaces without concerns about network isolation.

3. **None:**
- Disables networking for containers, enhancing security by isolating them from any connectivity.
- Functionality:
      - Results in a container with no network connectivity, ensuring isolation from other containers, host services, and the internet.
      - Enhances security by providing a sandbox environment for applications that do not require network connectivity.

4. **Overlay:**
- Enables distributed networking across multiple Docker hosts.
- Functionality:
      - Facilitates communication between containers on different hosts without OS-level routing.
      - Essential for Docker Swarm clusters or separate Docker Engine instances.
      - Necessary when creating distributed environments for high availability, allowing containers on different hosts to communicate directly.

5. **Macvlan:**
- An advanced option that presents containers as physical devices on the network.
- Functionality:
      - Assigns a unique MAC address to each container for differentiation.
      - Requires dedicating a host's physical interface to the virtual network.
      - Useful when containers need to emulate physical devices on the host's network, providing a more integrated presence.

6. **IPvLAN:**
- An advanced driver offering precise control over container IP addresses.
- Functionality:
      - Supports layer 2 and 3 VLAN tagging and routing for fine-grained network configuration.
      - Useful for integrating containerized services with an existing physical network.
      Provides advanced options for controlling container IP addresses, VLAN tagging, and routing, offering a high level of customization.


### Docker Networking Implementation
Docker utilizes the host's network stack to implement its networking system. It manipulates iptables rules to route traffic to containers, ensuring isolation between Docker networks and the host. Docker containers have their own network namespace and virtual network interfaces on the host.

#### Using Docker Networks

1. **Creating Networks**: Use docker network create to create a new network, specifying the driver (e.g., bridge).
```
docker network create demo-network -d bridge
```

2. **Connecting Containers to Networks**: Attach containers to a network using the --network flag.
```
docker run -it --rm --name container1 --network demo-network busybox:latest
```

3. **Using Host Networking**: Connect a container to the host network.
```
docker run -d --name nginx --network host nginx:latest
```

4. **Disabling Networking**: Disable networking for a container by attaching it to the none network.
```
docker run -it --rm --network none busybox:latest
```

5. **Removing Containers from Networks**: Use docker network disconnect to remove containers from networks.
```
docker network disconnect demo-network container2
```

#### Managing Networks

1. **List All Docker Networks**
```
docker network ls
```
2. **Remove a Network**
```
docker network rm network-name
```
3. **Prune Unused Networks**
```
docker network prune
```

#### Using Networks With Docker Compose
- Docker Compose automatically adds services to a shared bridge network.
- Define additional networks in the Compose file and connect services accordingly.


## Developing with Container
Developing with containers involves using containerization technologies, to streamline the development process, improve collaboration, and enhance application portability. 




## Docker Alpine
Docker Alpine represents the containerized adaptation of Alpine Linux, a Linux distribution celebrated for its exceptional lightweight nature and robust security features. Known for its minimalistic design and security-centric approach, Alpine Linux has become a favored option for containerized applications. Docker Alpine seamlessly blends the strengths of Alpine Linux—its lightweight and secure foundation—with the adaptability and user-friendly features inherent in Docker containers. This integration positions Docker Alpine as an outstanding preference for developers seeking to craft containerized applications that are both efficient and secure, offering ease of deployment and customization.


## Ubuntu Image/Container Commands

**Pull Ubuntu Latest Iamge**
```
docker pull ubuntu latest
```

**Create Ubuntu Container**
```
docker run -itd --name <container_name/id>  ubuntu /bin/bash
```
- NOTE: It will create a Ubuntu Container and will provide an interactive terminal

```
docker exec -it <container_name/id> /bin/bash
```
- NOTE: It will open the intreactive terminal of newly created container.

**Stop Ubuntu Container**
- To exit the interactive terminal of ubuntu container.
```
exit
```
- To close the ubuntu container

```
docker stop <container_name/id>
```

**Restart the Stoped Ubuntu Container**
- To start the ubuntu container
```
docker start <container_id/id>
```
- To enter the interactive terminal of running ubuntu container.
```
docker exec -it <container_id/id> /bin/bash
```
**Remove the Container**
```
docker rm <container_name/id>
```



## Docker Desktop Installation and Sign In Guide 

### Installa Docker Desktop On Linux-Ubuntu

1. **Update the System:**
```
sudo apt update
```
2. **Install Necessary Packages:**
```
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
```
3. **Add Docker GPG Key:**
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
4. **Set up Docker Repository:**
```
echo "deb [signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

5. **Update the Package Database:**
```
sudo apt update
```

6. **Install Docker Engine:**
```
sudo apt install -y docker-ce docker-ce-cli containerd.io
```
7. **Enable Docker Service:**
```
sudo systemctl enable --now docker
```
8. **Verify Docker Installation:**
```
sudo docker --version
```
- This should display the installed Docker version.

9. **Verify Docker is Running:**
```
sudo docker info
```
- This should provide information about the Docker daemon.

10. **Install Docker Desktop**

- [Click Here to Download Docker Desktop](https://docs.docker.com/desktop/install/ubuntu/)


### Signin Docker Desktop On Linux-Ubuntu

1. **Install Password Manager**
```
sudo apt-get install pass
```

2. **Generate `gpg-id_publik_key`**
```
gpg --generate-key
```
- Enter Email ID Register to Docker

3. **Initialize Password Manager**
```
pass init <generated_gpg-id_public_key>
```
- Now go to Docker Desktop and Singin