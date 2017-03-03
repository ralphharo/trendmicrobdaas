Ansible Trend Micro Agent
=========


[Documentation around these Ansible cloud modules ](http://docs.ansible.com/ansible/list_of_cloud_modules.html)

Requirements
------------


Role Variables
--------------

- `dsm_agent_download_hostname` - Hostname of the Deep Security manager	app.deepsecurity.trendmicro.com
- `dsm_agent_download_port` - The port to connect to the Deep Security manager on to download the agents. This is typically the same port as the admin web access	443
- `dsa_activation_hostname` - The hostname for the agents to communicate with once deployed.
- `dsa_activation_port` - The port to use for the agent heartbeat (the regular communication). For Marketplace AMI and software deployments, the default is 4118
- `tenant_id` - In a multi-tenant installation (like Deep Security as a Service), this identifies the tenant account to register the agent with
- `tenant_password` - In a multi-tenant installation (like Deep Security as a Service), this identifies the tenant account to register the agent with
- `policy_id` - The Deep Security ID assigned to the policy to apply to the agents on activation

Dependencies
------------

No dependencies on other Ansible roles

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Sample Playbook
      hosts: localhost
      connection: local
      gather_facts: False
      tags: security

    - roles:
         - { role: username.rolename }
