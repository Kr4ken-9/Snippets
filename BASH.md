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
---
### Get specific process maps (Source ?)

PID = process ID

Search = term to search for

Out = output file

`cat /proc/PID/maps | grep Search > Out`

---
### [Dump specific process memory](https://serverfault.com/questions/173999/dump-a-linux-processs-memory-to-file)

PID = process id

Out = output file

Begin = Beginning Memory Address

End = Ending Memory Address

`sudo gdb --batch --pid PID -ex "dump memory Out Begin End"`
