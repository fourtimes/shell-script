```bash
# Debugging the shell script with "-x"
shell script file name - test.sh

Run a script with debug output enabled:---

$ bash -x test.sh (or) bash --debug test.sh

Note:- 2
--------
#!/usr/bin/env bash
set -x   # Enable debugging
# some code here
set +x   # Disable debugging output.

```