# 1. Use an official Node.js image from Docker Hub as the base image
FROM node:14

# 2. Set the working directory inside the container
WORKDIR /usr/src/app

# 3. Copy package.json and package-lock.json from parent directory to the container
COPY ../package*.json ./

# 4. Install the dependencies specified in package.json
RUN npm install

# 5. Copy the rest of the application code to the container
COPY . .

# 6. Expose the port that the app will run on (usually 3000 for Node.js apps)
EXPOSE 3000

# 7. Start the application by running npm start
CMD ["npm", "start"]
