# [Command] _nginx deployment configuration create_

Create a configuration for an NGINX deployment

## Versions

### [2022-08-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL25naW54Lm5naW54cGx1cy9uZ2lueGRlcGxveW1lbnRzL3t9L2NvbmZpZ3VyYXRpb25zL3t9/2022-08-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/nginx.nginxplus/nginxdeployments/{}/configurations/{} 2022-08-01 -->

#### examples

- Single file Configuration Create
    ```bash
        nginx deployment configuration create --name default --deployment-name myDeployment --resource-group myResourceGroup --root-file /etc/nginx/nginx.conf --files "[{content:'aHR0cCB7CiAgICB1cHN0cmVhbSBhcHAgewogICAgICAgIHpvbmUgYXBwIDY0azsKICAgICAgICBsZWFzdF9jb25uOwogICAgICAgIHNlcnZlciAxMC4wLjEuNDo4MDAwOwogICAgfQoKICAgIHNlcnZlciB7CiAgICAgICAgbGlzdGVuIDgwOwogICAgICAgIHNlcnZlcl9uYW1lICouZXhhbXBsZS5jb207CgogICAgICAgIGxvY2F0aW9uIC8gewogICAgICAgICAgICBwcm94eV9zZXRfaGVhZGVyIEhvc3QgJGhvc3Q7CiAgICAgICAgICAgIHByb3h5X3NldF9oZWFkZXIgWC1SZWFsLUlQICRyZW1vdGVfYWRkcjsKICAgICAgICAgICAgcHJveHlfc2V0X2hlYWRlciBYLVByb3h5LUFwcCBhcHA7CiAgICAgICAgICAgIHByb3h5X3NldF9oZWFkZXIgR2l0aHViLVJ1bi1JZCAwMDAwMDA7CiAgICAgICAgICAgIHByb3h5X2J1ZmZlcmluZyBvbjsKICAgICAgICAgICAgcHJveHlfYnVmZmVyX3NpemUgNGs7CiAgICAgICAgICAgIHByb3h5X2J1ZmZlcnMgOCA4azsKICAgICAgICAgICAgcHJveHlfcmVhZF90aW1lb3V0IDYwczsKICAgICAgICAgICAgcHJveHlfcGFzcyBodHRwOi8vYXBwOwogICAgICAgICAgICBoZWFsdGhfY2hlY2s7CiAgICAgICAgfQogICAgICAgIAogICAgfQp9',virtual-path:'/etc/nginx/nginx.conf'}]"
    ```

- Multi-file Configuration Create
    ```bash
        nginx deployment configuration create --name default --deployment-name myDeployment --resource-group myResourceGroup --root-file /etc/nginx/nginx.conf --files "[{'content':'aHR0cCB7CiAgICB1cHN0cmVhbSBhcHAgewogICAgICAgIHpvbmUgYXBwIDY0azsKICAgICAgICBsZWFzdF9jb25uOwogICAgICAgIHNlcnZlciAxMC4wLjEuNDo4MDAwOwogICAgfQoKICAgIHNlcnZlciB7CiAgICAgICAgbGlzdGVuIDgwOwogICAgICAgIHNlcnZlcl9uYW1lICouZXhhbXBsZS5jb207CgogICAgICAgIGxvY2F0aW9uIC8gewogICAgICAgICAgICBpbmNsdWRlIC9ldGMvbmdpbngvY29uZi5kL3Byb3h5LmNvbmY7CiAgICAgICAgICAgIHByb3h5X3Bhc3MgaHR0cDovL2FwcDsKICAgICAgICAgICAgaGVhbHRoX2NoZWNrOwogICAgICAgIH0KICAgICAgICAKICAgIH0KfQ==','virtual-path':'/etc/nginx/nginx.conf'},{'content':'cHJveHlfc2V0X2hlYWRlciBIb3N0ICRob3N0Owpwcm94eV9zZXRfaGVhZGVyIFgtUmVhbC1JUCAkcmVtb3RlX2FkZHI7CnByb3h5X3NldF9oZWFkZXIgWC1Qcm94eS1BcHAgYXBwOwpwcm94eV9zZXRfaGVhZGVyIEdpdGh1Yi1SdW4tSWQgMDAwMDAwOwpwcm94eV9idWZmZXJpbmcgb247CnByb3h5X2J1ZmZlcl9zaXplIDRrOwpwcm94eV9idWZmZXJzIDggOGs7CnByb3h5X3JlYWRfdGltZW91dCA2MHM7','virtual-path':'/etc/nginx/conf.d/proxy.conf'}]"
    ```