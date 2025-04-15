# Step 1: Use an official Node.js runtime as a base image
FROM node:16

# Step 2: Set the working directory inside the container
WORKDIR /usr/src/app

# Step 3: Copy package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of the application files into the container
COPY . .

# Step 6: Expose the port that the application will run on (e.g., port 3000)
EXPOSE 3000

# Step 7: Command to run your app using Node.js
CMD ["node", "app.js"]
