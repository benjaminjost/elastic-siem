<p align="center">
    <img src="https://i2.wp.com/newtonpaul.com/wp-content/uploads/2020/12/Elastic_Siem_Blog.jpg?fit=1280%2C720&ssl=1" width="30%" alt="Elastic-SIEM"/>
</p>
<!-- Image source: https://newtonpaul.com/how-to-install-elastic-siem-and-elastic-edr/ -->

<h1 align="center">Elastic SIEM</h1>
<p align="center">Elastic-SIEM is a docker compose template to experiment with Elastic Security features such as SIEM and Elastic Endpoint Security.<br>
   <a href="https://www.elastic.co/security" title="Overview">Official Overview</a>
</p>  

<p align="center">
<a href="https://open.vscode.dev/benjaminjost/Elastic-SIEM" title="Open in VSCode">
<img src="https://img.shields.io/badge/Open%20in%20VSCode-%23007ACC?label=Code&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAC00lEQVQYGX3BX2iVZRwH8O/ze//t/NkcRzdXmzZzLLYMmyVJUFQgzkQoqOsgAtNu6jK6kqjbIqOErrrTCBUUbBTYuZCMoDE0FZLp3DpnZ9s55313znmf/89TEV1JfT5s6uIG5LlvsPTdKViK8fCzr2H8wGEw1UIpNqgUYkRx38Bajqorb08ateWT62l+NrtxBSH+R0KAdhhbaelqp7X26MTTE9ix58UzG83u+7/l9Q9DEMHKHE4JoNiHf0UEKIvH1zh+lMZsC+ME3ZzDt4FiUtz75NE3viXvDYpbx44AHkjXwShAQIBx7PkGD37NtdsWBAzWGihtYD2QtXsQxkmienu+9MRzl3Yf++wylQaLulWHIXolU76qjI8DBmil0drkn/qocFkbCwsGrbQilXUUz3vo3/PS7PiJL38pPDL10eb68nllHQIiGGfxe231BI1MvlceHk2lyGG9h/UeoSzoZ0i507Kx8mYyMjHth3ZOiz9uIehs+F5x63xN0Tvh0Ni13dMz4Fw8ZJwHwPA30k0JsVF/26SNW7ybQQgBN/wY9OCOzsp89ZD44etro4NbkFQi5FwY4xmMB4wHSDY5XCc7bZr3pmy2CksRFO/CVMb7KzMH5yLbPXDv/CmkLQkqlENjPYwFjAUoSsTPNqRjtjwc5XcXbvZuXv3YxmWoTsrCkcl9Q299/pMqDR9fnDsDFoc14xms97Deg0yaxDpWkKwwl9XW9qulGx9Abr6qPQPP2jCSozJ7/IuuCz9p318aZFEC4wHjAdK9ZEaz3lGh9CxjcR4UBwDevmDT5Re0gxZSw0gBjEy+y7V72ToGbTwsi2JigYMz/hJjACP8I0xAqld1zTtPaa1aCgGMFHCMYB3ASgOwCBLCXxhjeEBYANP5dVe/vddysSh9ABcVgP4IPG8vNL7/6vUQ/8kDcR+YyFf04sIMje6q6t5msnrl6kmRpWf1/ev4E5Tbl9R3VUZRAAAAAElFTkSuQmCC&style=flat-square" alt="Open in VSCode"/>
</a>

<a href="https://github.dev/benjaminjost/Elastic-SIEM" title="Open in VSCode Web">
<img src="https://img.shields.io/badge/Open%20in%20VSCode%20Web-%23007ACC?label=Code&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAC00lEQVQYGX3BX2iVZRwH8O/ze//t/NkcRzdXmzZzLLYMmyVJUFQgzkQoqOsgAtNu6jK6kqjbIqOErrrTCBUUbBTYuZCMoDE0FZLp3DpnZ9s55313znmf/89TEV1JfT5s6uIG5LlvsPTdKViK8fCzr2H8wGEw1UIpNqgUYkRx38Bajqorb08ateWT62l+NrtxBSH+R0KAdhhbaelqp7X26MTTE9ix58UzG83u+7/l9Q9DEMHKHE4JoNiHf0UEKIvH1zh+lMZsC+ME3ZzDt4FiUtz75NE3viXvDYpbx44AHkjXwShAQIBx7PkGD37NtdsWBAzWGihtYD2QtXsQxkmienu+9MRzl3Yf++wylQaLulWHIXolU76qjI8DBmil0drkn/qocFkbCwsGrbQilXUUz3vo3/PS7PiJL38pPDL10eb68nllHQIiGGfxe231BI1MvlceHk2lyGG9h/UeoSzoZ0i507Kx8mYyMjHth3ZOiz9uIehs+F5x63xN0Tvh0Ni13dMz4Fw8ZJwHwPA30k0JsVF/26SNW7ybQQgBN/wY9OCOzsp89ZD44etro4NbkFQi5FwY4xmMB4wHSDY5XCc7bZr3pmy2CksRFO/CVMb7KzMH5yLbPXDv/CmkLQkqlENjPYwFjAUoSsTPNqRjtjwc5XcXbvZuXv3YxmWoTsrCkcl9Q299/pMqDR9fnDsDFoc14xms97Deg0yaxDpWkKwwl9XW9qulGx9Abr6qPQPP2jCSozJ7/IuuCz9p318aZFEC4wHjAdK9ZEaz3lGh9CxjcR4UBwDevmDT5Re0gxZSw0gBjEy+y7V72ToGbTwsi2JigYMz/hJjACP8I0xAqld1zTtPaa1aCgGMFHCMYB3ASgOwCBLCXxhjeEBYANP5dVe/vddysSh9ABcVgP4IPG8vNL7/6vUQ/8kDcR+YyFf04sIMje6q6t5msnrl6kmRpWf1/ev4E5Tbl9R3VUZRAAAAAElFTkSuQmCC&style=flat-square" alt="Open in VSCode Web"/>
</a>
</p>

## Docker compose

Bringing up the stack: `sudo docker-compose up`  

As soon as the containers are ready, navigate to http://localhost:5601 and login with the following credentials  
**elastic : password**  

Cleanup: `sudo docker-compose down`  

## Beats

> "Beats is a free and open platform for single-purpose data shippers. They send data from hundreds or thousands of machines and systems to Logstash or Elasticsearch."
<p align="center">
<img src="https://www.elastic.co/guide/en/beats/libbeat/master/images/beats-platform.png" width="60%">
</p>

Here are two examples for Filebeat and Auditbeat.

### Filebeat

> "Filebeat is a lightweight shipper for forwarding and centralizing log data. Installed as an agent on your servers, Filebeat monitors the log files or locations that you specify, collects log events, and forwards them either to Elasticsearch or Logstash for indexing."  

- [Overview](https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-overview.html)
- [Download Filebeat client](https://www.elastic.co/downloads/beats/filebeat)
- [Install and configure Filebeat](https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation-configuration.html)
- [List of available modules](https://www.elastic.co/guide/en/beats/filebeat/7.11/filebeat-modules.html)

**TL;DR (short version)**
1) [Download client](https://www.elastic.co/downloads/beats/filebeat) (depending on the OS)
2) Enable modules `sudo ./filebeat modules enable auditd system`
3) Set up assets
   ```
   sudo chown root filebeat.yml \
   sudo chown -R root modules.d/ \
   sudo chown -R root modules/ \
   sudo ./filebeat setup -e
   ```  
4) Start Filebeat `sudo ./filebeat -e`
5) **Info**: Check the host, username and password configuration in the .yml file)

***

### Auditbeat

> "Auditbeat is a lightweight shipper that you can install on your servers to audit the activities of users and processes on your systems."  

- [Overview](https://www.elastic.co/guide/en/beats/auditbeat/current/auditbeat-overview.html)
- [Download Auditbeat client](https://www.elastic.co/downloads/beats/auditbeat)
- [Install and configure Auditbeat](https://www.elastic.co/guide/en/beats/auditbeat/current/auditbeat-installation-configuration.html)
- [List of available modules](https://www.elastic.co/guide/en/beats/auditbeat/current/auditbeat-modules.html)

**TL;DR (short version)**
1) [Download client](https://www.elastic.co/downloads/beats/auditbeat) (depending on the OS)
2) Set up assets
   ```
   sudo chown root auditbeat.yml \
   sudo ./auditbeat setup -e
   ```
3) Start Auditbeat `sudo ./auditbeat -e`
4) **Info**: Check the host, username and password configuration in the .yml file)

## Elastic Agents with Endpoint Protection

> "Elastic Agent is a single, unified way to add monitoring for logs, metrics, and other types of data to each host."

> "Fleet provides a web-based UI in Kibana to add and manage integrations for popular services and platforms, as well as manage a fleet of Elastic Agents."

[Overview of the endpoint security feature](https://www.elastic.co/endpoint-security/)  
[Install Elastic Endpoint integration](https://www.elastic.co/guide/en/security/current/install-endpoint.html)  

[Download Elastic Agent](https://www.elastic.co/downloads/elastic-agent)  
[Install Elastic Agent and enroll in Fleet](https://www.elastic.co/guide/en/fleet/current/elastic-agent-installation.html)

## Next configuration steps on the stack
- [Configure TLS](https://www.elastic.co/guide/en/elasticsearch/reference/current/configuring-tls.html#tls-http)
- [User authorization](https://www.elastic.co/guide/en/elasticsearch/reference/current/authorization.html)
- [API keys](https://www.elastic.co/guide/en/kibana/master/api-keys.html)

## Licence

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
