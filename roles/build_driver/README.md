## build_driver

This role will generate a SpecialResource CR from the template given by the
user.  It then applies the CR onto the cluster to kick start the driver builds.
Once the get_managed_clusters builds a list of OCP version from the
ManagedClusters CR, it builds a unique list of kernel version as some different
OCP version might have the same underlying kernel version.

## Requirements

SRO and Node Feature Discovery (NFD) have to be installed and properly functioning.

## Dependencies

This role depends on the get_managed_clusters role which will parse the
ManagedClusters CR on the ACM Hub cluster and build a list of OCP versions
under management.

## Example Playbook

    - hosts: provisioner
      ansible-playbook -i inventory.yml build_drivers.yml
