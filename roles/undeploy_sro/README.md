# undeploy_sro

This role un-deploys the SpecialResourceOperator.  It removes the namespace, the
operator group and the subscription from the cluster

# Requirements

The role requires a properly configured operator catalog so that the Operator
Lifecycle Manager can find and install the SRO package and its dependencies.


# Example Playbook

    - hosts: provisioner

ansible-playbook -i inventory.yml  undeploy_sro.yml

