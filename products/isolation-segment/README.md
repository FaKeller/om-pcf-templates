# Isolation Segment Configuration

Edit the configuration files and then execute the following command:

```bash
om -t <OPS_MANAGER_IP> -u <USER> -p <PASS> configure-product -n p-isolation-segment -p "$(cat isolation-segment.json)" -pn "$(cat isolation-segment-network.json)" -pr "$(cat isolation-segment-resources.json)" 
```