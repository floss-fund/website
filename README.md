# FLOSS/fund Website

This repository contains the source code for the FLOSS Fund website.

https://floss.fund

## Development Docs
### Build the Website with Zola using Docker

Follow these steps to build the website using Zola with Docker:

1. **Clone the Repository**
    ```sh
    git clone https://github.com/floss-fund/website.git
    cd website
    ```

2. **Run the Docker Container**
    ```sh
    docker run -u "$(id -u):$(id -g)" -v $PWD:/app --workdir /app ghcr.io/getzola/zola:v0.19.2 build
    ```

### Local Development

Make sure you have Docker installed and running on your machine before executing these commands.

4. **Serve the Website**
    ```sh
    docker run -u "$(id -u):$(id -g)" -v $PWD:/app --workdir /app -p 8080:8080 ghcr.io/getzola/zola:v0.19.2 serve --interface 0.0.0.0 --port 8080 --port 1024 --base-url localhost
    ```

5. **Access the Served Website**
    Open your browser and navigate to `http://localhost:8000` to view the live-reloaded website.
