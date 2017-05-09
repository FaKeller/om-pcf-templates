# PCF Configuration

Edit the configuration files and then execute the following command:

```bash
om -t <OPS_MANAGER_IP> -u <USER> -p <PASS> configure-product -n cf -p "$(cat pcf.json)" -pn "$(cat pcf-network.json)" -pr "$(cat pcf-resources.json)" 
```

---

## Troubleshooting

**Problem:**

```
configuring product...
setting properties
could not execute "configure-product": failed to configure product: request failed: unexpected response:
HTTP/1.1 400 Bad Request
Content-Length: 0
Connection: keep-alive
Content-Type: text/html; charset=utf-8
Date: Tue, 09 May 2017 14:20:52 GMT
Server: nginx/1.4.6 (Ubuntu)
Strict-Transport-Security: max-age=31536000
X-Request-Id: 5df23bed-e40d-4a68-8949-ab9eeb597a9b
X-Runtime: 0.005084
```

**Solution:** Split large JSON files to multiple small ones and issue a `configure-product` command for each smaller file.