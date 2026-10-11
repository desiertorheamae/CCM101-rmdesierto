# Laboratory 07: Mission Reflection

This laboratory helped me understand why monitoring is an important responsibility of a Cloud Operations Engineer. Checking the host server's resources is necessary even when containers appear to run properly because all containers depend on the underlying system. If RAM becomes insufficient or disk space runs out, applications may become slow, fail to save data, or stop responding. Establishing a baseline helps identify resource limitations before they affect users.

The `docker logs` command is useful when a user reports that they cannot log into a web application. By reviewing the logs, an engineer can identify failed requests, application errors, and other events that may explain the problem. For example, HTTP error responses can indicate that a requested page or resource is unavailable. Logs provide evidence that helps narrow down the possible cause instead of relying only on assumptions.

Log monitoring and metric monitoring provide different kinds of information. Logs describe individual events, such as successful requests and errors, while metrics show numerical measurements such as CPU usage, memory consumption, and network activity. Using both helps engineers understand what happened and whether resource limitations contributed to the issue.

Large enterprise companies may use monitoring platforms such as Prometheus and Grafana to manage thousands of containers. Prometheus can collect and store time-series metrics, while Grafana can display dashboards and trends that help teams identify unusual resource usage. Alerting systems can also notify engineers when performance reaches predefined limits.

My ability to troubleshoot Linux environments improved through using commands to inspect memory, disk space, running processes, container logs, and performance metrics. I also learned how to generate HTTP requests and intentionally produce a 404 error to test application behavior. Overall, this laboratory strengthened my understanding of system health, container observability, and the importance of collecting accurate evidence when diagnosing technical problems.
