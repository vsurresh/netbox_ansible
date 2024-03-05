# NetBox Ansible Automation

This repository contains Ansible playbooks for automating the setup of NetBox, including the creation of sites, devices, and connections.

## Prerequisites

Before running these playbooks, make sure you have Ansible installed on your machine. You also need access to a NetBox instance and have your NetBox API token ready.

## Getting Started

1. **Clone the repository**:

   ```bash
   git clone git@github.com:vsurresh/netbox_ansible.git

2. Set up your environment variables:

You'll need to export your NetBox URL and API token as environment variables. Replace http://your_netbox_url:port with your actual NetBox URL and your_netbox_api_token with your API token.
```
export NETBOX_URL=http://your_netbox_url:port
export NETBOX_TOKEN=your_netbox_api_token
```
3. Run the Playbooks:

The playbooks should be run in a specific order to ensure dependencies are correctly managed. Start with the site configuration, followed by devices, and finally, connections.
* ansible-playbook organization.yml
* ansible-playbook devices.yml
* ansible-playbook connection.yml

# Support
If you encounter any issues or have questions, please file an issue on GitHub, and I'll do my best to address it.