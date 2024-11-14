# Minecraft-Server-Docker-Compose

This project provides a complete setup for running a Minecraft server using Docker Compose. The server is configured with FABRIC, a lightweight and flexible modding platform that allows easy integration of custom mods. The server also supports local mods, enabling you to add, modify, and test mods without the need for manual file management on the server.

With this setup, you can create a Minecraft server environment that runs mods and plugins in an isolated and easily manageable way, without modifying system files or server settings.
What is this project?

This project allows you to run a customized Minecraft server within a Docker container, using Docker Compose to manage the necessary services. The server is configured with FABRIC, which is a fast and modular modding platform for Minecraft, and mods are managed locally, giving you full control over the installed mods.

By using this approach, you can easily create and manage your own custom Minecraft server with a set of mods tailored to your preferences.

# Features

   Docker Compose Setup: This project uses Docker Compose to automatically configure and launch the Minecraft server. All you need to do is modify the docker-compose.yml file to suit your needs.

   FABRIC Modding Platform: FABRIC is used to add additional mods to the server.
   
   Local Mods: This setup allows you to use custom mods stored locally on your machine. You can add these mods to a dedicated folder without having to manually upload them to the server each time.
   
   Minecraft Version Compatibility: You can use different versions of Minecraft, from the latest to older versions. You just need to adjust the version in the Docker configuration or the configuration files.
# Data directory

![level-vs-world](https://github.com/user-attachments/assets/b25b691e-afca-4de8-9ee8-063a6ca0470c)

# Installation and Setup

### 1. Clone the Repository

First, clone the repository to your local machine:
```
git clone https://github.com/username/Minecraft-Server-Docker-Compose.git
```
```
cd Minecraft-Server-Docker-Compose
```

### 2. Configure the Server

The main configuration file is docker-compose.yml. Open this file and modify it according to your preferences:

   Minecraft Version: Modify the line for the desired Minecraft version. Ensure it is compatible with FABRIC.

   Local Mods: Place your custom mods into the mods folder in the main project directory. Make sure the mods are compatible with the chosen version of Minecraft.

   Server Settings: Edit the server.properties file in the data folder to customize server settings, such as the port, difficulty level, and other game configurations.

### 3. Start the Server

After configuring the necessary files, you can start the server with Docker Compose:
```
docker-compose up -d
```
This will build and launch the Minecraft server container in the background, making it accessible on the configured port (default is 25565).

> [!NOTE] 
> Access the Server
>To connect to the Minecraft server, open the game and add a server using the local IP or the public IP
>```
>localhost:25565
>```

> [!IMPORTANT]
> You need to have the mod FABRIC API to the version of minecraft you are using
