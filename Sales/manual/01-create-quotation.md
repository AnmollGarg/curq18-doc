# Creating a Quotation

## Accessing the Sales Workspace

To open the Sales app in CURQ 18:

1. Click the main menu at the top of your screen.
2. Choose **Sales**.

The system opens directly to your quotations list with **My Quotations** selected by default. 

If you are already inside the Sales app, you can return to this list anytime by clicking **Orders** > **Quotations**.

---

## Starting a New Quotation

To start a new quotation, click the **New** button at the top left of the Quotations list view. This opens a blank quotation form.

### 1. Customer and Commercial Details

Begin by entering the name of your customer in the **Customer** field at the top of the form. This is a required field.

When you select a customer, the system automatically pulls data from their contact record:
* The **Invoice Address** and **Delivery Address** auto populate with the addresses saved for that customer. You can change them if this specific order requires different billing or shipping locations.
* The customer default **Pricelist** and **Payment Terms** fill in automatically.

Next, review and complete the remaining header fields:
* **Quotation Template**: Optionally choose a saved template. Selecting a template automatically fills in standard product lines, optional products, expiration date, terms and conditions, online signature and payment rules, and the invoicing journal.
  *(Refer to this guide to set up quotation templates)*
* **Quotation Date**: This field defaults to the current date and time when you created the quotation.
* **Expiration**: Select the date until which the quotation remains valid. If you selected a quotation template with a validity duration, this date calculates automatically.
* **Pricelist**: Confirm the currency and pricing rules applied to the products on this quote.
  *(Refer to this guide to set up pricelists)*
* **Payment Terms**: Specify the payment schedule, such as Immediate Payment or 30 Days.

### 2. Adding Products on the Order Lines Tab

Under the **Order Lines** tab, specify the items or services being quoted. 

To add an item, click **Add a product**. In the **Product** field, search for and select your product:
* Selecting a product automatically fills in its **Description**, **Unit of Measure**, **Unit Price**, and applicable **Taxes**.
* Enter the desired amount in the **Quantity** field.
* If you sell in bulk packages, select a **Packaging** type and specify the **Packaging Quantity**. The system then updates the total unit quantity accordingly.
* If you want to give a price reduction on a specific line, enter a percentage in the **Discount** field.
* The **Amount** field calculates the line total automatically.

You can also use the following controls:
* Click **Catalog** to open a side panel where you can browse products visually with photos and add items with one click.
* Click **Add a section** to create header categories that divide your quote into clear visual groups.
* Click **Add a note** to insert custom text or instructions that will print directly on the customer document.

### 3. Offering Optional Products

Open the **Optional Products** tab to offer additional accessories, upgrades, or services.

Items listed here do not affect the quotation total initially. Instead, when the customer views the quotation online through the customer portal, they can choose to add these optional items to their order before signing.

Click **Add a product** to select the item, enter the suggested **Quantity**, and set the **Unit Price** or **Discount**.

### 4. Configuring Other Info

Open the **Other Info** tab to review delivery, commercial, and accounting settings:

#### Sales
* **Salesperson**: The internal employee in charge of this deal.
* **Sales Team**: The sales group credited for the revenue.
* **Company**: The company branch managing the transaction.
* **Online Signature**: Check this box to require the customer to sign electronically on the portal to confirm the order.
* **Online Payment**: Check this box to require an online prepayment before the order confirms. You can specify whether to collect a partial deposit or the full amount.
* **Customer Reference**: Enter the purchase order number or reference provided by the customer.
* **Tags**: Add descriptive labels to help filter and find this order later.
* **Print Variant Grids**: Check this box if you want the PDF quote to display a matrix table for products with multiple size or color options.

#### Invoicing
* **Fiscal Position**: Adjusts taxes automatically if the customer is located in another country or qualifies for tax exemption.
* **Invoicing Journal**: The accounting journal where invoices generated from this order are posted.

#### Delivery
* **Shipping Weight**: Displays the total physical weight calculated from all ordered products.
* **Warehouse**: The storage facility responsible for picking, packing, and shipping the items.
* **Incoterm**: Select international trade rules, such as EXW, FOB, or CIF.
* **Incoterm Location**: The city, port, or facility named in the trade rule agreement.
* **Shipping Policy**: Choose whether to ship products as soon as each item is available, or wait until all items are ready for a single shipment.
* **Delivery Date**: The promised arrival or shipment date agreed upon with the customer.

#### Tracking
* **Source Document**: Displays the lead, opportunity, or previous document that generated this quotation.
* **Campaign, Medium, and Source**: Marketing fields used to trace the channel or campaign that brought in this sale.
