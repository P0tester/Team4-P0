# Yu_Timothy_Bradburn_Kenneth_P0
Project0 Repository for Timothy Yu and Kenneth Bradburn
Update as of 10/13/2021

Robot adds a vendor as long as the information given to the robot in an Excel sheet matches a specific format. Our rationale being if this is for a store or webpage that information could be translated from HTML easily.

Excel sheet format for vendors (vendor_inventory sheet):

| Vendor | Item | Item Cost | Item Discount | Item Count |
| ------ | ---- | --------- | ------------- | ---------- |

Robot can run an order that accounts for discounts and does not pull the order of an item if there is not enough in stock. Our reasoning is to not fulfill an order for a singular item in that order if we can not fully deliver. IE: A person wants 2 tires and 1 water. If our inventory shows 1 tire and 1 water. The Client will receive the water and we will have a printout showing that we could not fill the order of the tires. That way we could "delay" a shipment of the tires to them until we get an updated inventory. So they will be charged for the water and that will be processed but they will get a notice that tires will need to be restocked.

As requested a Run All has been added to run reports for all clients in ascending order by Order Number. (First come First served)

Robot has updated add client and shopping list with full automation as long as client name is provided. Order Number is added and is modular.

Excel sheet format for clients (individual client sheets with the client name):

| Name | Email | Order | Quantity |
| ------ | ---- | --------- | ------------- |


There is a method for updating the inventory now with a new shipment. The format has to account for items that we are not getting in and they have to be represented with a 0 number of incoming products.

Excel sheet format for incoming shipments (sheet: incoming_shipment):

| Vendor | Item | Item Count| 
| ------ | ---- | --------- |

Robot has a process to Email clients, based on their interests, if there are discounts on the items they have in their shopping list. Note: Currently has the email process commented out and needs enabled. The reason for this is if you do it too many times you can get blocked.

## MVP
- [x] Robot should be able to take client shopping lists and place orders on the appropriate vendors.
- [x] Robot should record the total expense of each shopping trip for each client.
- [x] Robot should be able to record any items that were out of stock or not found.
- [x] Robot should be able to add clients to the existing client list and take in their shopping order.
- [x] Robot should be able to add more vendors in the existing vendor collection.
- [x] Robot should be able to take in account discounts noted by the vendors.

## Stretch Goals
- [ ] Sending emails to clients about their shopping order
- [x] Notify clients about vendor discounts/sales
- [ ] Email vendors about out of stock items
- [x] Restock inventory for vendors
- [ ] Any other extra features that would improve UX

## Tech Stack
- UiPath Studio
# Team4-P0
