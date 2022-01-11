## deploy_pre_requisites

This role deploys some of the requirements needed to run the playbooks with the sample driver.

## Dependencies

podman command must be installed.

## Example Playbook

    - hosts: provisioner
      ansible-playbook -i inventory.yml deploy_prerequisites.yml
