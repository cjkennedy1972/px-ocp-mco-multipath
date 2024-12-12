# px-ocp-mco-multipath

Applying the two YAML files in this repo creates an OpenShift MachineConfig to enable multipathd and configure it to ignore locally attached devices and adds Pure Storage's recommended UDEV rules.

** Updated Nov. 5th 2024**
- Latest multipath.conf for Pure Storage FlashArrays

** Updated Dec. 12th, 2024**
- Added UDEV Rule to YAML
- Removed "find_multipaths:" from the multipath.conf file and base64 value
- added machineconfiguration.operator.yaml to allow adding multipath.conf without a reboot, now just restarts the service on the node.

