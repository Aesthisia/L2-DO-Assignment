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

**Verify the Fix:**

 - After resolving the error inside the container, you should be able to see "Welcome to Aesthisia."

### Success Criteria:

**Error Diagnosis:**

   - Identify whether the "403 Forbidden" error is caused by misconfiguration within the Docker container.

**Resolution Details:**

  - Provide a clear explanation of the root cause of the error and the steps taken to resolve it, including any adjustments made to permissions or other necessary changes.

**Verification of Fix:**
  - Confirm that after resolving the error, accessing the application displays "Welcome to Aesthisia" without encountering the "403 Forbidden" error.

**Documentation:**
  - Document any modifications made inside the container for future reference and clarity.

---
