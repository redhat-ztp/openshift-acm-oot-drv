## validate_sro

This role checks that the SRO and NFD are running and in good health. It checks
that the necessary pods are present and in good state.

## Requirements

SRO and NFD have to be installed and properly functioning.

## Example Playbook

    - hosts: provisioner
      ansible-playbook -i inventory.yml build_drivers.yml

