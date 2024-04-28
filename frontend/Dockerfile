# Set the lightweight base image
FROM node:21-alpine
# Set the working directory to /app
WORKDIR /app
# Copy the rest of the application code
COPY . .
# Install dependencies
RUN npm i
# Copy the .env.dicker file to .env.local
COPY .env.docker .env.local
# Expose port 5173 for the Node.js application
EXPOSE 5173
# Define the default command to run the application in development mode
CMD ["npm", "run", "dev", "--", "--host"]
