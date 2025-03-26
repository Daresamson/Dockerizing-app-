# Step 1: Set Up the Node.js Application
![Screenshot (83)](https://github.com/user-attachments/assets/25e8b53b-3d8d-42f9-ab38-62edb13bbf62)

# Step 2: Write a Dockerfile
# Use official Node.js image as base
FROM node:20

## Create app directory
WORKDIR /usr/src/app

## Install app dependencies
COPY package*.json ./
RUN npm install

## Copy app source
COPY . .

## Expose port 3000
EXPOSE 3000

## Start the app
CMD ["node", "app.js"]
![Screenshot (84)](https://github.com/user-attachments/assets/eac73e42-e89c-4468-a917-f3be7e0f16a4)

## Check the app running at: http://localhost:3000
![Screenshot (82)](https://github.com/user-attachments/assets/83c1e9ba-4fa7-42ec-91ce-99666dfadd19)

# Step 3: Push to Docker Hub
![Screenshot (89)](https://github.com/user-attachments/assets/adc9e753-ca5b-4982-b481-8c228a3e6660)
![Screenshot (90)](https://github.com/user-attachments/assets/00cead9c-6716-4fb5-8385-58a73cf2b1af)





