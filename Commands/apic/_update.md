# [Command] _apic update_

Update an instance of an Azure API Center service.

## Versions

### [2024-03-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5hcGljZW50ZXIvc2VydmljZXMve30=/2024-03-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.apicenter/services/{} 2024-03-01 -->

#### examples

- Update service details
    ```bash
        apic update -g contoso-resources -n contoso
    ```

- Update Service With System Assigned Identity Example
    ```bash
        apic update -g contoso-resources -n contoso --identity '{type:systemassigned}'
    ```
