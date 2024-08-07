# [Command] _support in-subscription tickets update_

Update API allows you to update the severity level, ticket status, advanced diagnostic consent, secondary consent, and your contact information in the support ticket.<br/><br/>Note: The severity levels cannot be changed if a support ticket is actively being worked upon by an Azure support engineer. In such a case, contact your support engineer to request severity update by adding a new communication using the Communications API.

## Versions

### [2024-04-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L3N1cHBvcnR0aWNrZXRzL3t9/2024-04-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/supporttickets/{} 2024-04-01 -->

#### examples

- Update support ticket severity.
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --severity "moderate"
    ```

- Update support ticket status.
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --status "closed"
    ```

- Update support ticket customer contact details properties
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --contact-additional-emails "xyz@contoso.com" "devs@contoso.com" --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-us" --contact-last-name "Bar" --contact-method "phone" --contact-phone-number "123-456-7890" --contact-timezone "Pacific Standard Time"
    ```

- Update advanced diagnostic consent of a support ticket
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --advanced-diagnostic-consent "Yes"
    ```

- Update secondary consent of a support ticket
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --secondary-consent "[{type:VirtualMachineMemoryDump,user-consent:No}]"
        support in-subscription tickets update --ticket-name "TestTicketName" --secondary-consent [0].type="VirtualMachineMemoryDump" --secondary-consent [0].user-consent="No"
        support in-subscription tickets update --ticket-name "TestTicketName" --secondary-consent [0]="{type:VirtualMachineMemoryDump,user-consent:No}"
    ```
