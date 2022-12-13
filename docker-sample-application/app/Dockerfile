FROM node:12-alpine
RUN apk add --no-cache python2 g++ make
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000

### Execution steps
## Start your container using the docker run command and specify the name of the image
# docker build -t getting-started .
## Start an app container. Running the new container in “detached” mode (in the background) and creating a mapping between the host’s port 3000 to the container’s port 3000. 
# docker run -dp 3000:3000 getting-started
