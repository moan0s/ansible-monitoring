# Monitoring via Ansible


This playbook can deploy a full monitoring stack with

* Prometheus
* Grafana
* Node Exporter
* Alertmanager
* Uptime Kuma (self built)
and possibly

* a MQTT broker
* InfluxDB
* Telegraf

# Usage

Install everything with

```shell
ansible-playbook -i inventory/hosts setup.yml --tags=all
```


# Troubleshooting

On Ubuntu I had to install `fontconfig` manually when setting up grafana.

# Restore

When you somehow lost your vars file (that is not under version control) you can find it under `/monitoring/vars.yml`. on the server.
You can deactivate this behaviour by setting `vars_yml_snapshotting_enabled: false`