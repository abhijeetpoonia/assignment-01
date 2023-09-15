FROM ubuntu

WORKDIR /app

# Copy the entire application directory into the container
COPY . .

# Install Node.js and npm
RUN apt-get update && apt-get install -y nodejs npm

# Install application dependencies
RUN npm install


# Build the application
RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
