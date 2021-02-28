---
id: 5f6c1202-1572-484b-b397-02e2b81aa5ad
title: Tensorboard
desc: ''
updated: 1611408774771
created: 1611408597020
---

# TensorBoard

Tensorboard does not render direct in Google AI Notebooks, a simple workaround is to SSH into the machine from your local, this involves two steps.

1. Run TensorBoard on the VM:
```
$ tensorboard --port=7000 --logdir logs
```

2. SSH into the machine:
```
$ gcloud beta compute ssh --zone "{your zone}" "{your instance name}" --project "{your project name}" -- -L 7000:localhost:7000
```

You can not access the TensorBoard UI from your own machine on `localhost:7000`