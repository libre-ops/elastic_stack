Elastic Stack Ansible role
==========================

This is an Ansible role for provisioning a self-hosted **ElasticStack server** (ElasticSearch, Kibana, etc), and provisioning the corresponding **log/metric shippers** on clients (MetricBeat, FileBeat, etc).

There's quite a lot of configuration options for setting up Elasticstack. The files in the [example directory](example) provide a rough guide,
including some options to try it out in `development` before setting it up for `production`. 

Alpha version notice: everything except Logstash is working and thoroughly tested. Logtash isn't actually needed for simple use cases.

For security in production, use of **CA certificates** is recommended. See role: https://github.com/libre-ops/ca_keys

ElasticStack requires OpenJDK. See role: https://github.com/libre-ops/open_jdk
