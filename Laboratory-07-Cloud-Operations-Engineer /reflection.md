# Mission 7: The Cloud Operations Engineer

## Mission Reflection

### 1. Why is it important to check the host server's resources even if your containers are running perfectly?

It is important to check the host server because containers still depend on the physical or virtual server's CPU, memory, and storage. Even if the containers are working properly, the server could run out of resources when traffic increases. Checking the host's resources helps identify possible problems before they affect the application.

### 2. If a user complains that they cannot log into a web application, how would the `docker logs` command help you solve the problem?

The `docker logs` command allows me to see what is happening inside the container. I can check the logs for errors, failed requests, or other messages related to the login problem. This can help me identify whether the issue is coming from the application or another part of the system.

### 3. What is the difference between monitoring logs and monitoring metrics?

Logs provide detailed records of events that happened in an application, such as successful requests and errors like HTTP 404. Metrics provide numerical information about system performance, such as CPU usage, memory usage, and network activity. Logs help explain what happened, while metrics help show how the system is performing.

### 4. How do you think large enterprise companies monitor thousands of containers at the same time?

Large companies can use monitoring tools such as Prometheus and Grafana to collect and display information from many containers. Prometheus can collect metrics from the infrastructure, while Grafana can present the information through dashboards. This allows Cloud Operations teams to monitor many systems from one place and quickly identify performance problems.

### 5. How has your ability to troubleshoot Linux environments improved?

My ability to troubleshoot Linux environments has improved because I learned how to use command-line tools to check system resources, running processes, application logs, and container performance. I also learned that troubleshooting should be based on actual evidence instead of guessing. Using commands such as `top`, `docker logs`, and `docker stats` gives me useful information for finding and understanding problems.
