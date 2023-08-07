<div align="center">
  <h1><strong>Unveiling the Docker Symphony: <br>Crafting a Secure and Dynamic Infrastructure</strong></h1>
</div>


<p align="center">
  <img src="https://dspelaez.github.io/img/thumbnails/docker-art.png" alt="docker banner"/>
</p>

## About  :

"*Inception*" is your passport to Docker mastery at 1337. Our mission? To construct a service infrastructure using Docker, choreographed by the ever-mysterious Docker Compose.
Within this mission, a focal point emerges. A sentinel, **NGINX**, stands guard, accessible through port 443. It unveils a network shrouded in enigma, revealing hidden services. Here, nginx meets **WordPress**, guided by **php-fpm**, and whispers secrets to **MariaDB**, the data custodian.

Yet, the SAGA continues! WordPress** and **MariaDB** inscribe their legacy within dedicated volumes, epitomizing data's endurance.
Step into "Inception" – where Docker's power orchestrates a symphony of services. Welcome to a journey where containers hold secrets, networks weave connections, and volumes etch persistence. Join us on this voyage of Docker discovery and mastery.

----
### Architecture :
- A Docker container that contains NGINX with TLSv1.2 or TLSv1.3 only.
- A Docker container that contains WordPress + php-fpm (it must be installed and configured) only without nginx.
- A Docker container that contains MariaDB only without nginx.
- A volume that contains your WordPress database.
- A second volume that contains your WordPress website files.
- A docker-network that establishes the connection between your containers.
<p align="center">
  <img src="https://user-images.githubusercontent.com/54292953/147146268-a616f39a-3f16-41f8-80c9-db5494c3dfe7.png" alt="img" width="450"/>
</p>

### Docker-related terminology :
**Docker** : Docker is an open-source platform that automates the process of developing, shipping, and running applications in isolated environments called containers. Containers package applications, libraries, dependencies, and configurations, ensuring consistent behavior across different environments.

**Container** : A container is a standalone, lightweight, and executable software package that includes everything needed to run a piece of software, including the code, runtime, system tools, and libraries. Containers isolate applications from their environment, providing consistency and portability.

**Image** : An image is a template that defines the environment and runtime for a container. It consists of a snapshot of a filesystem and configuration settings. Images are used to create container instances, ensuring consistent deployment across various stages of development.

**Dockerfile** : A Dockerfile is a text file that contains instructions for building a Docker image. It defines the base image, sets up the environment, installs dependencies, and configures the application. Dockerfiles enable reproducible and automated image creation.

**Docker Compose** : Docker Compose is a tool that allows you to define and manage multi-container Docker applications using a simple YAML file. It enables you to specify services, networks, volumes, and their interactions in a single configuration.

**Volume** : A volume is a persistent data storage mechanism provided by Docker. Volumes enable containers to store and share data with the host machine and other containers, even if the container is stopped or removed.

**Network** : A Docker network is a virtual network that facilitates communication between containers, enabling them to interact securely. Networks can be used to isolate containers, group them by project, or simulate complex network topologies.

**Registry** : A Docker registry is a repository for Docker images. It serves as a centralized location to store, share, and distribute Docker images. Docker Hub is a popular public registry, but you can also set up private registries for internal use.

**Compose File** : A Compose file is a YAML file used to define services, networks, and volumes for a Docker Compose application. It specifies the configuration and relationships of the containers within the application.

**Service** : In Docker Compose, a service refers to a container and its configuration settings defined in the Compose file. Services define how a container should be built, run, and connected to other containers.

**Orchestration** : Orchestration is the management and coordination of multiple containers to work together as a single application. Docker orchestration tools like Docker Swarm and Kubernetes enable automated deployment, scaling, and management of containerized applications.
