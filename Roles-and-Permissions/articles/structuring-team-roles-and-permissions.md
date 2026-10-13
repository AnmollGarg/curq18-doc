# Structuring Team Roles and Access Permissions

Discover how a multi-company business organizes team permissions across departments, prevents accidental system configuration changes, streamlines employee onboarding, and safeguards corporate records in CURQ 18.

---

### 1. The Real-World Challenge

As organizations expand across multiple branches and departments, unmanaged user permissions quickly lead to operational errors and compliance risks:

1. **Accidental System Changes**: Granting employees full administrative rights allows well-meaning team members to alter global pricelists, delete accounting journals, or modify invoice layouts.
2. **Confidentiality and Margin Exposure**: Sales representatives viewing competitor accounts, internal purchase costs, or draft invoices meant for other departments.
3. **Offboarding Security Gaps**: Departing employees retaining active system access because user accounts were not promptly deactivated.

This guide illustrates how **Apex Industrial Technologies** and its branch **Apex Industrial (Midwest)**, managed by system administrator **Sarah Jenkins**, design a clean role hierarchy in CURQ 18.

---

### 2. Department Role Architecture

Sarah Jenkins avoids assigning full **Administrator** privileges to operational staff. Instead, management defines standardized job profiles across the organization:

* **Commercial Sales Representative**:
  * **Sales**: *User: Own Documents Only* (can create quotes and orders for assigned clients only).
  * **Invoicing**: *Blank (None)* (cannot issue or view accounting invoices).
  * **Inventory**: *Blank (None)* (cannot edit stock levels).
* **Sales Team Lead**:
  * **Sales**: *User: All Documents* (full visibility across the sales team pipeline).
  * **Invoicing**: *Invoicing* (can create customer invoice drafts).
  * **Point of Sale**: *User* (operates retail trade counter registers).
* **Warehouse Coordinator**:
  * **Inventory**: *User* (validates receipts, delivery orders, and internal transfers).
  * **Sales**: *Blank (None)*.
  * **Invoicing**: *Blank (None)*.
* **Accounting Specialist**:
  * **Invoicing**: *Invoicing* (processes customer invoices, registers vendor bills, and records payments).
  * **Bank**: *Validate bank account* (authorized to verify supplier bank account numbers).
  * **Inventory**: *Blank (None)*.
* **System Administrator**:
  * **Administration**: *Settings* (reserved strictly for Sarah Jenkins and core IT management).

---

### 3. Step 1: Create the User Profile and Contact Record

When hiring a new sales team member, **David Miller**:

1. Open **Settings** from the main dashboard.
2. Navigate to **Users & Companies** → **Users**.
3. Click the blue **New** button in the upper-left corner.
4. Enter `David Miller` in the **Name** field.
5. In the **Email Address** field, enter `david.miller@apexindustrial.com`.
6. *(Optional)* Click the camera avatar icon to upload their employee photo.

CURQ automatically creates an associated partner card in the Contacts directory, linking David's personal contact details to his system user login.

---

### 4. Step 2: Assign Department Access Levels and Multi-Company Visibility

Under the **Access Rights** tab on David Miller's user card:

1. In the **SALES** section, locate the **Sales** field and select **User: Own Documents Only**.
2. Confirm all other non-sales modules (such as **Inventory**, **Project**, and **Administration**) remain set to **Blank (None)**.
3. Under the **Multi Companies** section:
   * **Allowed Companies**: Select `Apex Industrial Technologies` and `Apex Industrial (Midwest)`.
   * **Default Company**: Select `Apex Industrial Technologies`.
4. Click **Save** in the top action bar.

David can now log quotes and manage his assigned customers across the authorized branches, but cannot view quotes created by other representatives, alter warehouse stock, or view company financial statements.

---

### 5. Step 3: Configure Communication and Timezone Preferences

To prevent notification noise and ensure timestamps match local working hours:

1. On David Miller's user card, switch to the **Preferences** tab.
2. In the **Localization** section, verify the **Language** is set to `English (US)` and set the **Timezone** to `America/Chicago`.
3. In the **Notification** field, choose **Handle in CURQ** so daily system notifications stay organized inside the internal chatter bell icon rather than cluttering his email inbox.
4. In the **Email Signature** box, enter his official corporate signature block:
   ```text
   David Miller | Commercial Sales Representative
   Apex Industrial Technologies
   david.miller@apexindustrial.com | +1 (312) 555-0144
   ```
5. Click **Save**.

---

### 6. Step 4: Dispatch the Secure Onboarding Invitation

1. With the user profile verified, click **Send an Invitation Email** in the top action bar.
2. CURQ dispatches an automated onboarding email containing a single-use token link.
3. David Miller opens the link, sets his confidential password, and signs in to CURQ for the first time.
4. The user status badge in the top right automatically updates from **Never Connected** to **Confirmed**.

---

### 7. Step 5: Promote or Transition Roles

When David Miller is promoted to Sales Team Lead after several months:

1. Navigate to **Settings** → **Users & Companies** → **Users** and open `David Miller`.
2. Under the **Access Rights** tab:
   * Change **Sales** from **User: Own Documents Only** to **User: All Documents**.
   * Change **Invoicing** from **Blank (None)** to **Invoicing**.
3. Click **Save**.
4. Advise David to refresh his web browser. His top navigation menu immediately updates to include the Invoicing application and complete visibility across team sales orders.

---

### 8. Step 6: Securely Offboard Departing Employees

When an employee (such as `Alex Taylor`) leaves the company, security compliance requires immediate revocation of access without losing historical records:

1. Open the user card in **Settings** → **Users & Companies** → **Users** and open `Alex Taylor`.
2. Click the **Actions** gear icon at the top of the form.
3. Select **Archive** from the dropdown menu and confirm the prompt.
4. An **Archived** ribbon displays across their profile card.
5. The employee login session is terminated immediately, preventing any further system access.
6. All historical quotations, confirmed orders, chatter messages, and activity audit trails authored by Alex remain fully preserved in the database.

---

### 9. Key Benefits for Business Operations

* **Eliminated Configuration Accidents**: Restricting administrative rights prevents accidental modifications to global tax settings, pricelists, or document layouts.
* **Clear Role Boundaries**: Team members only see the apps and records necessary for their daily work, reducing interface clutter and preventing data leakage.
* **Instant Offboarding Compliance**: Archiving a user blocks system login instantly while preserving full audit history for accounting and compliance reviews.
* **Smooth Scalability**: Standardizing department role profiles allows management to onboard new hires in less than two minutes.

