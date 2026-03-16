Here is an essential Docker Cheat Sheet in Markdown format, covering images, containers, and orchestration. 
🖼️ Image Management
Images are the read-only templates used to create containers. 
Docker Docs
Docker Docs
Command 	Description
docker images	List all locally stored images
docker build -t [name] .	Build an image from a Dockerfile in the current directory
docker pull [image]	Download an image from a registry like Docker Hub
docker rmi [image]	Remove a specific image from local storage
docker tag [src] [target]	Create a new tag for an existing image
docker push [image]	Upload an image to a registry
📦 Container Lifecycle
Containers are the running instances of your images. 
Docker Docs
Docker Docs
 +1
Command 	Description
docker ps	List only currently running containers
docker ps -a	List all containers (running and stopped)
docker run -d [image]	Run a container in the background (detached mode)
docker stop [id]	Stop a running container
docker start [id]	Start a previously stopped container
docker rm [id]	Delete a stopped container
docker logs -f [id]	View and follow real-time logs for a container
🛠️ Interactive & Debugging
Use these to "enter" or inspect what's happening inside a container. 
Docker Docs
Docker Docs
 +1
Command 	Description
docker exec -it [id] bash	Open an interactive terminal inside a running container
docker inspect [id]	View detailed JSON configuration of a container or image
docker stats	Show live resource usage (CPU, Memory) for all containers
docker cp [src] [dest]	Copy files between the host and a container
🧩 Docker Compose (Multi-container) 
Used for managing applications with multiple services (e.g., App + Database). 
AWS in Plain English
AWS in Plain English
 +1
Command 	Description
docker compose up -d	Start all services in the background
docker compose down	Stop and remove all containers, networks, and images defined in the file
docker compose logs -f	View aggregated logs for all services
🧹 System Cleanup
Command 	Description
docker system prune	Remove all unused data (stopped containers, unused networks/images)
docker image prune	Specifically remove "dangling" (untagged) images
Would you like a sample Dockerfile to see how to package a basic application into an image?





undefined
undefined
undefined
13 sites
CLI Cheat Sheet - Docker Docs
Page 1 * CLI Cheat Sheet. * Build an Image from a Dockerfile. Build an Image from a Dockerfile without the cache. * docker build -

Docker Docs

Docker Commands Cheat Sheet: Complete Reference
3 Mar 2026 — Table_title: Docker Cheatsheet: Quick Command Reference Table_content: header: | Command | What it does | row: | Command: docker p...

buddy.works

Docker Cheat Sheet: Essential Commands Every Developer Should ...
25 Jul 2025 — 🚀 Key Docker CLI Commands * docker run – Start a container from an image. * docker ps – List running containers. * docker exec -i...

Medium

Show all
Here is a sample Dockerfile for a basic Python application. You can save this text as a file named Dockerfile (with no file extension) in your project folder. 
Microsoft Learn
Microsoft Learn
 +1
dockerfile
# 1. Use an official base image (e.g., Python, Node, or Alpine)
FROM python:3.9-slim

# 2. Set the working directory inside the container
WORKDIR /app

# 3. Copy dependencies file to the container
COPY requirements.txt .

# 4. Install any needed packages
RUN pip install --no-cache-dir -r requirements.txt

# 5. Copy the rest of the application code
COPY . .

# 6. Expose the port the app runs on (e.g., 8080)
EXPOSE 8080

# 7. Define the command to run the application
CMD ["python", "app.py"]
Use code with caution.

🧱 Breakdown of Instructions
FROM: Sets the starting point for your image, usually an official operating system or language runtime.
WORKDIR: Defines the "home" directory inside the container where all following commands will run.
COPY: Transfers files from your computer into the container's filesystem.
RUN: Executes commands while building the image, such as installing software or updates.
EXPOSE: Acts as documentation, telling users which port the application listens on.
CMD: The final command that starts your application when the container launches. 
Docker Docs
Docker Docs
 +6
🚀 How to Build and Run
Once your Dockerfile is ready, use these commands in your terminal: 
Build the image: docker build -t my-app .
Run the container: docker run -p 8080:8080 my-app 
