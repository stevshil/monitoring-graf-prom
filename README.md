# Monitoring Lab Prometheus & Grafana

This lab is specifically set up for Grafana and Prometheus.  Applications in this are Wordpress and Petclinic with a MariaDB database backing both applications.

All application containers are running node-exporter and process-exporter internally.

## Application Containers

### Wordpress

To access wordpress;

- http://localhost:1180

Adminstrator page;

- http://localhost:1180/wp-admin
  - Username: admin
  - Password: admin123

### Petclinic

- http://localhost:1080

### MariaDB database

Username: root
Password: petclinic

## Monitoring Containers

### Grafana

- http://localhost:3000
  - Username: admin
  - Password: admin

### Prometheus

- http://localhost:9090

### dbmon

This is a mysql-exporter which provides metrics as a side car from MariaDB database to Prometheus, rather than it running directly in the database container.