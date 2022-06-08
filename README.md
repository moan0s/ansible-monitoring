# Monitoring via Ansible


This playbook can deploy a full monitoring stack with

* Prometheus
* Grafana
* Node Exporter
* Alertmanager

and possibly

* a MQTT broker
* InfluxDB
* Telegraf

# Usage

Install everything with

```shell
ansible-playbook -i inventory/hosts setup.yml --tags=all -K
```


# Troubleshooting

On Ubuntu I had to install `fontconfig` manually when setting up grafana.

