## Getting Started

First you need to have docker install locally

You can check out [guide to install docker](https://docs.docker.com/get-docker/)

To run application for development:

```bash
# To build an image
docker build -t sliver-ape/front-end .

# Start development server
docker run -it  -v ${PWD}:/app -v /app/node_modules -p 3000:3000 -e CHOKIDAR_USEPOLLING=true sliver-ape/front-end

```