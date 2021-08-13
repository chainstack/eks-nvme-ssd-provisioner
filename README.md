# eks-nvme-ssd-provisioner

The eks-nvme-ssd-provisioner will format to XFS and mount NVMe SSD disks on EKS nodes. This is needed to make the [sig-storage-local-static-provisioner](https://github.com/kubernetes-sigs/sig-storage-local-static-provisioner) work well with EKS clusters. The eks-nvme-ssd-provisioner will create a raid0 device if multiple NVMe SSD disks are found.
