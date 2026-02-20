# PostgreSQL HA Lab

## Inventory
- Master: 192.168.5.133
- Replica: 192.168.5.134

## Setup
ansible-playbook playbook.yml

## Load testing
sudo -u pgbench pgbench -i -U pgbench bench
sudo -u pgbench pgbench -c 10 -T 60 -U pgbench bench