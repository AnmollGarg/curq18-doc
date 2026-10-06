# Dashboard Groups Configuration

Create and organize dashboard groups, define sidebar category hierarchy, adjust display sequences, and manage group spreadsheets and permissions in CURQ 18.

---

### 1. Overview of Dashboard Groups

Dashboard groups serve as top-level category containers in the left navigation sidebar of the **Dashboards** app *(such as **Sales**, **Finance**, **Logistics**, and **Services**)*.

Organizing dashboards into structured groups allows administrators to:
* Keep business metrics neatly categorized by department or functional domain.
* Control the vertical display sequence of categories in the sidebar using drag-and-drop handles.
* Directly attach and manage spreadsheets, security access groups, and publishing status within each group.

---

### 2. Navigating to Dashboards Configuration

To view and manage dashboard groups:

1. Open the **Dashboards** app from the main menu.
2. In the top navigation bar, click **Configuration**.
3. Select **Dashboards**.

![Dashboards Configuration dropdown highlighting the Dashboards menu item](images/dashboard-configuration-menu.png)

4. The **Dashboards** list displays all active category groups *(such as Sales, Finance, Logistics, Services, Marketing, Website, and Human Resources)*.

---

### 3. Reordering Groups in the Navigation Sidebar

The top-to-bottom sequence in the list view directly governs the vertical order of categories in the Standard Dashboards navigation sidebar:

1. Navigate to **Dashboards > Configuration > Dashboards**.
2. Click and hold the drag handle (`⠿`) at the far left edge of any row.
3. Drag the group row up or down to your desired position and release to save the new order automatically.

![Dashboards list view showing category groups and drag-and-drop handles](images/dashboards-list-view-reorder.png)

---

### 4. Creating a New Dashboard Group and Registering Spreadsheets

To create a new departmental category and attach dashboards to it:

1. In the **Dashboards** list view, click the **+ New** button at the top left.
2. In the form view, enter the group title in the top name field *(such as `Human Resources`)*.
3. In the **Spreadsheets** tab, click **Add a line** to register dashboards within this category:
   * **Name**: Enter the title of the individual dashboard *(such as `Employees` or `Recruitment`)*.
   * **Group**: Select a security access group to restrict viewing rights to authorized roles *(such as `Human Resources / Officer`)*. Leave empty to allow general access.
   * **Company**: Select a specific company if this dashboard should only appear in multi-company environments.
   * **Is Published**: Check this box to make the dashboard live and visible to end users.
   * **Active**: Ensure the record is active.

![Dashboard group creation form showing group name and Spreadsheets configuration tab](images/dashboard-group-form-spreadsheets.png)

4. Click the cloud save icon or navigate back to apply the new category and its spreadsheet dashboards.

---

### 5. Verifying Groups in the Navigation Sidebar

Once created and published, the category group appears in the Standard Dashboards sidebar navigation:

1. In the top navigation bar, click **Dashboards**.
2. Verify that the new category heading and its underlying dashboards appear in the left sidebar in your configured sequence.

![Standard Dashboards navigation sidebar displaying configured category groups](images/dashboard-sidebar-groups-display.png)
