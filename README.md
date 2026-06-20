NOTES
=====

Init whitelist
--------------

```sh
WHITELIST=YOUR_PATH
systemctl list-units --type=service --state=running --no-legend | awk '{print $1}' | sort > ${WHITELIST}
```