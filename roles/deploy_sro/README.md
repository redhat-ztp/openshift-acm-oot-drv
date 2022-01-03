## deploy_sro

This role deploys the SpecialResourceOperator.  It adds a namespace, an
operator group and a subscription to the cluster

## Requirements

The role requires a properly configured operator catalog so that the Operator
Lifecycle Manager can find and install the SRO package and its dependencies.


## Example Playbook

    - hosts: provisioner
      ansible-playbook -i inventory.yml  deploy_sro.yml

