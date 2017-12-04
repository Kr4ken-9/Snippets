### [Convert to uppercase](https://www.cyberciti.biz/faq/linux-unix-shell-programming-converting-lowercase-uppercase/)

`"${VAR^^}"`

Example:

```bash
MIX=AeIoU

echo -n "${MIX^^}"
```
---
### [Get hash w/out file name](https://superuser.com/questions/273435/clean-up-sha256sum-output)

`HASH="$(sha256sum FILE | head -c 64)"`

Example:

```bash
echo -n "fat" > test

HASH="$(sha256sum test | head -c 64)"

echo HASH
```
