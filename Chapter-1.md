## Concepts

## Federation


## Two Tracks
Developer
Operations

## Reference Architecture

3-5 Server Agents (m5.large / m5.2xlarge)
1 Leaders and rest are followers
Raft consensus in choosing a leader

Min 3 Client Agents (Agent sizing depends on your needs)

Multiple Regions -> Multiple Clusters 

Clusters don't share jobs, clients, state or data.

Single Cluster -> Single Region

## HashiCorp Stack

Packer 
TF
Consul
Vault
Vagrant

## Nomad Modes
Server
Client
Dev Modes

long running agent

## Configuration Files
- mode, resources, location
Multiple Files (contents are merged. Newer values overwrite previous values)

## Server Mode

Manage the cluster
Shares tasks with other sever members
nomad server command.

Manage all clients in the cluster

server stanza 


## Client Mode
Expected to join a Nomad Cluster
Runs the assigned jobs
Managed by the server agents

nomad node command
