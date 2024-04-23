# DevOps Assignment

## Assignment Description:

### Task 1: Dockerizing a Node.js App with Multi-stage Dockerfile
- **Objective:** Dockerize a simple Node.js application using a multi-stage Dockerfile.
- **Steps:**
  1. Set up a basic Node.js application.
  2. Write a multi-stage Dockerfile for the Node.js application to ensure efficient deployment in a production environment.
  3. Utilize a custom port by defining it in the Nginx configuration to manage incoming requests efficiently.

### Task 2: Deploying the Dockerized App in Kubernetes
- **Objective:** Deploy the Dockerized Node.js application in a Kubernetes cluster (Minikube or any other cluster).
- **Steps:**
  1. Set up a Kubernetes cluster (Minikube or any other cluster).
  2. Write Kubernetes deployment file for deploying the Node.js application.
  3. Create a Kubernetes service file for port forwarding.

### Task 3: Implementing Horizontal Pod Autoscaler (HPA)
- **Objective:** Implement Horizontal Pod Autoscaler (HPA) for the deployed application.
- **Steps:**
  1. Write HPA YAML file for configuring autoscaling.
  2. Define resource limitations (CPU and RAM) for the deployed application pods.
  3. Set up load testing tools to send multiple requests to the application.
  4. Monitor the performance of the application and observe the behavior of HPA.

### Task 4: Submission Requirements
- **Objective:** Upload the complete codebase, including Kubernetes deployment manifests, to a public GitHub repository.
- **Steps:**
  1. Create a public GitHub repository for the project.
  2. Upload all the necessary files including Dockerfile, Kubernetes deployment manifests, and HPA YAML file to the repository.
  3. Capture a screenshot demonstrating the scaling behavior of the HPA during the load test, showcasing scaling up the replicas.
  4. Update the repository's README.md file with documentation of the project setup.

## Success Criteria:
- **Functional Kubernetes Deployment:**
  - The Node.js application should be successfully deployed and accessible within the Kubernetes cluster.
  - Verify the deployment using `kubectl get pods` and `kubectl get services` commands.
- **HPA Configuration:**
  - Horizontal Pod Autoscaler (HPA) should be configured to automatically scale the application based on resource usage.
  - Verify the HPA configuration using `kubectl get hpa` command.
- **Successful Load Test Execution:**
  - Execute a load test on the deployed Node.js application.
  - Capture a screenshot demonstrating the scaling behavior of the HPA during the load test.

---