---
id: e1270b08-3e4d-4724-af7d-53ef73a3b614
title: CLI
desc: ''
updated: 1614158006759
created: 1610883840988
---

# CLI Commands

List files with sizes in a directory

```bash
# Specify MBs (10^6 bytes)
$ ls -l --block-size=MB

# Human readable sizes
$ ls -lh
```

Delete a directory

```bash
# -r deletes everything inside `recursively`
$ rm -r DIR_NAME
```

Keep program running when SSH closed

```bash
$ screen
# Now run your long lived command
# When returning, to access the same process:
$ screen -r
```