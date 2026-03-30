# Ansible Automation Lab

## Overview
This project demonstrates building modular, scalable automation using Ansible in a simulated multi-node environment.

## Architecture
- Control Node: Ubuntu VM
- Target Nodes: Docker containers
- Automation Tool: Ansible

## Features
- Role-based automation (webserver role)
- Apache installation and configuration
- Container-aware service management (no systemd)
- Idempotent playbooks

## Project Structure

ansible-lab/
├── inventory/
├── playbooks/
├── roles/
│   └── webserver/
├── ansible.cfg

## Key Concepts Demonstrated
- Ansible roles and modular design
- YAML-based automation
- Conditional task execution
- Process-based service management for containers
- Infrastructure automation patterns

## How to Run

```bash
ansible-playbook playbooks/apache.yml
