# get_managed_clusters

This role builds a list of OCP version from the ManagedClusters CR.
For each OCP version found, it pulls the corresponding Driver toolkit image to
find out its kernel version.

# Requirements

- SRO and NFD have to be installed and properly functioning.
- An ACM cluster with a set of SNOs under management.

# Example Playbook

    - hosts: provisioner

ansible-playbook -i inventory.yml build_drivers.yml

