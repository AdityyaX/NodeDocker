# Node.js Dockerized Application

This repository contains a Node.js application Dockerized using Docker. It demonstrates how to containerize a Node.js application for easy deployment and distribution.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/node-dockerized.git
   ```

2. Build the Docker image:

   ```bash
   docker build -t node-dockerized .
   ```

3. Run the Docker container:

   ```bash
   docker run -d -p 3001:3001 node-dockerized
   ```

4. Access the application:

   Open your web browser and visit `http://localhost:3001` to access the Node.js application running inside the Docker container.

## Dockerfile

The `Dockerfile` in this repository is used to build the Docker image for the Node.js application. It includes the following steps:

- Use the official Node.js image as the base image.
- Set the working directory inside the container.
- Copy the application files into the container.
- Install application dependencies using `npm install`.
- Expose port 3001 to allow external access to the application.
- Start the Node.js application using `node index.js`.

## Usage

- Modify the `index.js` file or add new files to the application.
- Rebuild the Docker image after making changes:

  ```bash
  docker build -t node-dockerized .
  ```

- Stop the running container:

  ```bash
  docker stop <container-id>
  ```

- Start a new container with the updated image:

  ```bash
  docker run -d -p 3001:3001 node-dockerized
  ```

## Resources

- [Docker Documentation](https://docs.docker.com/)
- [Node.js Documentation](https://nodejs.org/en/docs/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
