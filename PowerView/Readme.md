How to add a PowerView Hub device to the TapHome application

1. Connect a PowerView Hub device to your local network. In PowerView app, set static IP address of the Hub (Hub->Hub Info->Static IP->Use Static IP=ON)
2. In the Taphome app create Packet parser interface or open the existing one.
3. Click the “Add from template” button and choose the PowerView Hub template.
4. Find out an IP address of the PowerView Hub.
5. Enter the IP address.
6. Click the “Create” button.
7. Find out an ID of your roller/blinds by entering the URL http://(IP_address)/api/shades in any browser, where (IP_address) is the IP address of your PowerView Hub. Attribute “shadeIds” contains an ID.

Example:
> "shadeIds":[7348]

Warning: there can be more than one ID in the “shadeIds” field if you have more than one roller/blinds.

8. Open Service Settings of the created device in the TapHome app.
9. Enter the ID number into the field Device ID.
