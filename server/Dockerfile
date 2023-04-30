# Use the official Node.js image as the base image
FROM node:14-alpine

# Set the working directory to /app
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the application code
COPY . .

# Set environment variables for Atlas MongoDB and S3
ENV MONGODB_URI='mongodb+srv://Adityaanaparthi:Aditya1234@cluster1.xk0ypyn.mongodb.net/test'
ENV AWS_ACCESS_KEY_ID='AKIA4IT3MYK6XCMZPA54'
ENV AWS_SECRET_ACCESS_KEY='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'
ENV S3_BUCKET_NAME=capstone546

# Expose the port on which the application will run
EXPOSE 5000

# Start the application
CMD ["npm", "start"]
