---
id: 26ed9307-c898-430d-8f9b-2dbdf6930798
title: Vms
desc: ''
updated: 1611924271224
created: 1611916760034
---

# GCP VMs

## SSH

You can `ssh` into an AI notebook VM, just like any other, and we can forward the port to view the notebooks locally:

```bash
export PROJECT_ID="PROJECT_ID"
export ZONE="ZONE"
export INSTANCE_NAME="INSTANCE_NAME"

gcloud compute ssh \
    --project $PROJECT_ID \
    --zone $ZONE \
    $INSTANCE_NAME -- -L 8080:localhost:8080
```

Very similar to how to access a TensorBoard running on the VM: [[ml.tf.tensorboard]]