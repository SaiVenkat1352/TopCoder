# Use the official Node.js base image as the foundation
FROM node:20-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json for installation
COPY package*.json ./

# Install dependencies
RUN npm install 

# Copy the .env file into the container


# Copy the rest of the application code to the container
COPY . .

# Expose the port your app runs on (typically 3000)
EXPOSE 3000

# Set environment variables from the .env file
ENV PORT=3000
ENV JWT_SECRET=$%&*^$#@!*&
ENV SUBMISSION_THRESHOLD=3
ENV SCORE_PENALTY=15
ENV mongo_url=mongodb+srv://meesalavenkatasai9:EVu1xYzLpQlxDTPi@cluster0.90cpd.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
ENV CLIENT_URL=https://new-online-judge-8y8o.vercel.app

# Define the command to run the application
CMD ["node", "Server.js"]
