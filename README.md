- Objective:
Create an ELK (Elasticsearch, Logstash, Kibana) stack that allows a user to search by IP and Status code in nginx access logs.

- Approach:
* Setup an nginx instance
* Write the access logs (10,000 lines minimum) to disk
* Take the nginx access logs from disk
* Parse the fields out in real time
* Send them into an ELK stack that you setup
* Add a template to Elasticsearch so that the source IP is stored as an IP type and status code is stored as an integer
* Kibana should use the timestamp of the log entry for display and not the timestamp of Elasticsearch insertion

- Requirements:
Elasticsearch 2.0+
Kibana 4.0+
Github repo for any code/config written, *commit very often* with descriptions
Kibana must have authentication of some sort
Use of logstash is optional
No existing docker solutions (i.e. DockerHub images)

- Resources:
http://brewhouse.io/blog/2014/11/04/big-data-with-elk-stack.html
https://www.nginx.com/blog/monitoring-nginx-plus-statistics-elk/
