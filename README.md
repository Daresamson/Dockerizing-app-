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
![Screenshot (92)](https://github.com/user-attachments/assets/f1586315-2ff3-4cc5-becf-f4b762a3bef6)


# Step 4: Push to AWS ECR
![Screenshot (101)](https://github.com/user-attachments/assets/d224da4d-0df1-497b-802e-b0ec1241229e)


# Step 6: Automate the Process with GitHub Action

![Screenshot (99)](https://github.com/user-attachments/assets/4b3bb323-fc69-4f1c-9ce1-c345753c4262)

![Screenshot (98)](https://github.com/user-attachments/assets/66d8aa2b-952f-4abd-9e75-8a73084be984)

![Screenshot (96)](https://github.com/user-attachments/assets/dc42a826-9229-46f5-a9ef-faacb5e2b93d)











