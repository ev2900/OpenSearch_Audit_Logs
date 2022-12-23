# OpenSearch Audit Logs
[OpenSearch audit logs](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/audit-logs.html) can be used to help determine the search request loads on a given domain. 

Audit logs are grouped into 2 different categories 
* REST layer - communication with HTTP clients ie. all HTTP requests that arrive at the cluster
* Transport layer - communication between nodes

In this example we can explore how to enable REST layer audit logs and find search operations within these logs

1. Enable audit logs

Navigate to the OpenSearch page on the AWS console, select your domain, select the logs section and then enable audit logs
