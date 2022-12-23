# OpenSearch Audit Logs
[OpenSearch audit logs](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/audit-logs.html) can be used to help determine the search request loads on a given domain. 

Audit logs are grouped into 2 different categories 
* REST layer - communication with HTTP clients ie. all HTTP requests that arrive at the cluster
* Transport layer - communication between nodes

In this example we can explore how to enable REST layer audit logs and find search operations within these logs

1. Enable audit logs - AWS Console

Navigate to the OpenSearch page on the AWS console, select your domain, select the logs section and then enable audit logs

<img width="600" alt="os-deleted-document-api" src="https://github.com/ev2900/OpenSearch_Audit_Logs/blob/main/README/OpenSearch_Enable_Audit_Logs.PNG">

Follow the prompts to create a CloudWatch log group and access policy

2. Enable audit logs - OpenSearch Dashboard

Log into the OpenSearch dashboard, navigate to the security page, then to the audit logs section. Enable the REST layer audit. Enable logging of the REST body if desired.

<img width="600" alt="os-deleted-document-api" src="https://github.com/ev2900/OpenSearch_Audit_Logs/blob/main/README/OpenSearch_Enable_REST_Audit_Logs.PNG">

Logging on the REST layer is now enabled. Make several requests to the OpenSearch domain to generate logs

3. View REST audi logs in CloudWatch
