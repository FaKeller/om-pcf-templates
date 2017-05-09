# BOSH Configuration

To configure BOSH, adjust all values in the `.json` configuration files in the respective directory of your IaaS.
If you have finished editing the configuration files, execute the following command in the respective directory of your IaaS to set the BOSH configuration in your OpsManager instance:

```bash
om -t <OPS_MANAGER_IP> -u <USER> -p <PASS> configure-bosh -i "$(cat iaas.json)" -d "$(cat director.json)" -s "$(cat security.json)" -a "$(cat az.json)" -n "$(cat networks.json)" -na "$(cat network-assignment.json)"
```