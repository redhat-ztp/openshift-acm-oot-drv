## deploy_drivers

This role deploys the built container drivers onto the relevant SNOs.  It
creates a PlacementRule, a PlacementBinding and a Policy that wraps the
MachineConfig template given by the user.

## Requirements

The driver containers are built and pushed to the external registry.

## Role variables

A state variable is passed to either add or remove all the objects that this
role uses. An 'absent' state will remove all the objects while a 'present'
state will add all the objects.

## Example Playbook

    - hosts: provisioner
      ansible-playbook -i inventory.yml -e "state=absent" deploy_drivers.yml
      ansible-playbook -i inventory.yml -e "state=present" deploy_drivers.yml

