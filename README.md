# Kafka Cluster Ansible Playbook

This Ansible playbook automates the installation and configuration of an Apache Kafka cluster on a Debian-based homelab environment. The setup includes one ZooKeeper node for coordination and three Kafka worker nodes for message processing and storage.

## Overview

- **ZooKeeper Node**: 1
- **Kafka Broker Nodes**: 3

## Prerequisites

- Debian-based operating system on all nodes
- Ansible installed on the control machine
- SSH access to all nodes with appropriate permissions

## Directory Structure

├── inventory
├── playbook.yml
├── README.md
└── roles
    └── kafka
        ├── handlers
        │   └── main.yaml
        ├── tasks
        │   └── main.yml
        ├── templates
        │   └── kafka_server.properties.j2
        └── vars
            └── main.yaml