# Docker Assignment: Troubleshooting "403 Forbidden" Error

## Objective:
   Resolve the "403 Forbidden" error encountered when accessing a Dockerized application.

### Steps:

 **Pull the Docker Image:**
 
  - Pull the Docker image sarveshsd/assignment.

**Run the Docker Container:**

 - After pulling the image, run the container with the following command:
      
       docker run -d -p 3000:3000 sarveshsd/assignment

**Troubleshoot the "403 Forbidden" Error:**

 - Upon accessing the application through the browser, troubleshoot and resolve the error.

**Solve the Issue:**

 - Identify the cause of the error, which might be related to the NGINX configuration.

**Verify the Fix:**

 - After resolving the error inside the container, you should be able to see "Welcome to Aesthisia."

### Reference:

- Here’s the reference to the Dockerfile used for building the Docker image sarveshsd/assignment:
  
      FROM node:19 AS build
      WORKDIR /app
      COPY package.json .
      RUN npm install
      COPY . .
      RUN npm run build
      EXPOSE 3000
      
      # Stage 2: Runtime stage
      FROM nginx:latest
      COPY --from=build /app/build /usr/share/nginx/html
      COPY nginx.conf /etc/nginx/conf.d/default.conf
      EXPOSE 3000
      CMD ["nginx","-g","daemon off;"]


### Success Criteria:

**Error Diagnosis:**

   - Identify whether the "403 Forbidden" error is caused by misconfigured NGINX settings or any other issues within the Docker container.

**Resolution Details:**

  - Provide a clear explanation of the root cause of the error and the steps taken to resolve it, whether it involves modifying NGINX configuration, adjusting permissions, or any other necessary changes.

**Verification of Fix:**
  - Confirm that after resolving the error, accessing the application displays "Welcome to Aesthisia" without encountering the "403 Forbidden" error.

**Documentation:**
  - Document any modifications made to the NGINX configuration or inside the container for future reference and clarity.

---