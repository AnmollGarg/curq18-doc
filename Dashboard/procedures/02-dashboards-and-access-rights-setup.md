# Dashboards and Access Rights Setup

Create standard dashboards, assign them to dashboard groups, define display ordering, and configure user security access groups in CURQ 18.

---

### 1. Overview of Dashboard Setup and Access Rights

In CURQ 18, standard dashboards are centrally managed definitions that compile live operational figures into responsive visual workspaces. 

Setting up dashboards through the configuration backend allows administrators to:
* Assign individual dashboards to specific **Dashboard Groups** *(such as placing `Invoicing` under `Finance`)*.
* Define the exact sorting sequence of dashboards within a group.
* Restrict sensitive business dashboards *(such as executive profit metrics or financial statements)* to authorized security groups using **Access Groups**.
* Customize or edit underlying spreadsheet templates that drive the KPI metrics and graphs.

---

### 2. Navigating to Dashboards Configuration

To view and manage all configured dashboards:

1. Open the **Dashboards** app from the main menu.
2. In the top navigation bar, click **Configuration**.
3. Select **Dashboards**.

![Dashboards Configuration dropdown highlighting Dashboards](images/dashboard-configuration-dashboards-menu.png)

4. The **Dashboards** list displays all configured dashboards, their assigned dashboard groups, display sequences, and defined access restrictions.

![Dashboards list view displaying configured dashboards, groups, and access rights](images/dashboards-list-view-configuration.png)

---

### 3. Creating a New Dashboard Record

To register and configure a new dashboard:

1. In the **Dashboards** list view, click the **New** button at the top left.
2. Complete the configuration fields on the form:
   * **Name**: Enter a descriptive title for the dashboard *(such as `Quarterly Sales Targets` or `Executive Cash Flow`)*.
   * **Dashboard Group**: Select the category group where this dashboard will be nested in the left sidebar *(such as `Sales` or `Finance`)*.
   * **Sequence**: Enter a numerical display sequence. Lower values place the dashboard higher within its parent group in the sidebar.

![Dashboard configuration form showing Name, Dashboard Group, and Sequence fields](images/dashboard-form-create-general.png)

---

### 4. Configuring Security and Access Groups

By default, any dashboard without access group restrictions is visible to all users who have access to the Dashboards application. To restrict visibility for sensitive operational or financial data:

1. On the dashboard configuration form, locate the **Access Groups** field.
2. Click the dropdown menu to select the user security groups permitted to view this dashboard *(such as `Accounting / Accountant`, `Sales / Administrator`, or `Administration / Settings`)*.
3. You can select multiple user groups if cross-functional visibility is required.
4. Users who do not belong to at least one of the specified groups will not see this dashboard or its category heading in their navigation sidebar.

![Dashboard configuration form highlighting the Access Groups security field](images/dashboard-form-access-groups-field.png)

5. Click the save icon to commit the security settings.

---

### 5. Editing the Underlying Spreadsheet

Standard dashboards are driven by CURQ Spreadsheet definitions that calculate metrics and render chart widgets:

1. On the dashboard configuration form, click the **Edit in Spreadsheet** smart button or action at the top.
2. The full CURQ Spreadsheet interface opens, allowing you to:
   * Adjust data sources, formulas, and live record filters.
   * Customize chart dimensions, bar colors, and KPI scorecards.
   * Add new pivot tables or list insertions.
3. Save the spreadsheet and return to the Dashboards app to inspect live data rendering.

![Dashboard configuration view highlighting the Edit in Spreadsheet button](images/dashboard-edit-in-spreadsheet-action.png)

---

### 6. Verifying User Visibility

To confirm that access rights have been applied correctly:

1. Log in with an account that does **not** have the assigned security group privileges.
2. Open the **Dashboards** app and verify that the restricted dashboard does not appear in the left sidebar.
3. Log in with an authorized user account and confirm that the dashboard displays and populates live data as expected.

![Comparison showing restricted sidebar visibility based on user access groups](images/dashboard-access-rights-verification.png)
