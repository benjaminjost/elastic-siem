# Elastic SIEM

Elastic-SIEM is a docker compose template to experiment with Elastic Security features such as SIEM and Elastic Endpoint Security.  
[Overview](https://www.elastic.co/security)  

## Docker compose

Bringing up the stack: `sudo docker-compose up`  

As soon as the containers are ready, navigate to http://localhost:5601 and login with the following credentials  
**elastic : password**  

Cleanup: `sudo docker-compose down`  

## Beats

"Beats is a free and open platform for single-purpose data shippers. They send data from hundreds or thousands of machines and systems to Logstash or Elasticsearch."
<p align="center">
<img src="https://www.elastic.co/guide/en/beats/libbeat/master/images/beats-platform.png" width="60%">
</p>

Here are two examples with Filebeat and Auditbeat.

### Filebeat

- [Download Filebeat](https://www.elastic.co/downloads/beats/filebeat)
- [Installing the Filebeat shipper](https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation-configuration.html) 
- [Full list of available modules](https://www.elastic.co/guide/en/beats/filebeat/7.11/filebeat-modules-overview.html)

Short version:
1) Enable modules `sudo ./filebeat modules enable auditd system`  
2) Set up assets 
   ```
   sudo chown root filebeat.yml \
   sudo chown -R root modules.d/ \
   sudo chown -R root modules/ \
   sudo ./filebeat setup -e
   ```  
3) Start Filebeat `sudo ./filebeat -e`

***

### Auditbeat

- [Download Auditbeat](https://www.elastic.co/downloads/beats/auditbeat)
- [Installing the Auditbeat shipper](https://www.elastic.co/guide/en/beats/auditbeat/current/auditbeat-installation-configuration.html) 

Short version:
1) Set up assets 
   ```
   sudo chown root auditbeat.yml \
   sudo ./auditbeat setup -e
   ```
2) Start Auditbeat `sudo ./auditbeat -e`

## Elastic Agents with Endpoint Protection

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
