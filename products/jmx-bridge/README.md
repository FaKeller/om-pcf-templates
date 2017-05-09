# JMX Bridge Configuration

Edit the configuration files and then execute the following command:

```bash
om -t <OPS_MANAGER_IP> -u <USER> -p <PASS> configure-product -n p-metrics -p "$(cat jmx-bridge.json)" -pn "$(cat jmx-bridge-network.json)" -pr "$(cat jmx-bridge-resources.json)" 
```