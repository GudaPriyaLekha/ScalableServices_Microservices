# Stage 1: Build the Angular app
FROM node:20 as builder

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the Angular project files
COPY . .

# Build the Angular app
RUN npm run build -- --prod

# Debugging: Check if the dist folder exists
RUN ls -al /app/dist/library-management-app

# Stage 2: Serve the app with Nginx
FROM nginx:alpine

# Copy the Angular build output to Nginx's default directory
COPY --from=builder /app/dist/library-management-app /usr/share/nginx/html

# Expose the default Nginx port
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
