# Admin Quick Start Guide - Configuring the Department Document Drive

The administrator must create the Department Document Drive and configure the folders within it by following the steps below.

1. **Create Department Document Drive**: Create a company-wide Department Document Drive for use across the entire organization.
2. **Create Folders by Department**: Create folders by department within the company-wide Department Document Drive. Department folders can be **configured in a multi-level structure identical to the Organization Chart** or **simplified to a single depth by team unit**, as shown in the figure below.            &#x20;

<div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162858.png" alt=""><figcaption></figcaption></figure></div>

3. **Set Folder Permissions**: Set permissions for each department folder so that only employees of that department can access it. This guide explains permission settings separately for the case of creating single-depth folders by team unit and the case of creating folders following the multi-level department structure.

{% hint style="warning" icon="square-poll-horizontal" %}
Refer to the following when choosing the folder configuration method for the company-wide Department Document Drive.

* **Multi-level structure identical to the Organization Chart**: A method of configuring folders hierarchically in the same way as the company's Organization Chart. This structure can reflect the organizational system as-is, and security can be enhanced by subdividing document access permissions by parent/child department.
* **Single-depth structure by team unit**: A method of configuring each team, the lowest level of the Organization Chart, as a single-depth folder. The simple structure makes it easy to set up and manage, and it is particularly suitable for small organizations. It also has the advantage of being able to respond quickly to changes such as organizational restructuring.
{% endhint %}

### <mark style="color:$primary;">Creating the Department Document Drive</mark>

The steps to create the company-wide Department Document Drive are as follows.

1. Select the **Personnel Management – Organization Chart – Organization chart management** menu on the admin webpage, then launch the **Organization Chart Editor**.
2. In the department/group panel on the left side of the Organization Chart Editor, select the department where you want to create the Document Drive. To create a company-wide Department Document Drive, select the site name (in the example below, **MYCOMPANY**).&#x20;

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162918.png" alt=""><figcaption></figcaption></figure>

3. Click **Create Team Documents Drive** in the top toolbar.
4. In the 'Create Team Documents Drive' window, set the capacity and name of the Department Document Drive, then click the **Create** button.

<div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162929.png" alt=""><figcaption></figcaption></figure></div>

5. Once the Department Document Drive is created, users can view the Department Drive in Windows Explorer.&#x20;

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162940.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="square-poll-horizontal" %}
The **DOC\_EXPORT** and **RECYCLER** folders are special folders automatically created when the Department Document Drive is created.
{% endhint %}

### <mark style="color:$primary;">Creating Folders by Department</mark>

To create Department Document Drive folders for the first time, you must log in to the webpage with the **Service Administrator** account.

1. Click the ![](../.gitbook/assets/img_006.png) button to the right of the account name in the upper right of the webpage, then select **Execute agent** to launch the Windows Agent.&#x20;

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162951.png" alt=""><figcaption></figcaption></figure>

* If the Windows Agent is not installed on the PC, click the **OK** button in the installation guide message to proceed with installation.
* After installation is complete, select the **Execute agent** menu again to launch the Windows Agent.



2. Click the Department Drive in Windows Explorer, then use **New – Folder** from the Explorer menu to create folders.&#x20;

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162958.png" alt=""><figcaption></figcaption></figure>

3. The folders created under the Document Drive are displayed. The following is an example of creating folders in the same structure as the Organization Chart above.

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163006.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:$primary;">Setting Folder Permissions</mark>

#### Setting Folder Permissions in a Single-Depth Structure

When team unit folders are created as shown in the figure below, folder permissions must be set as in the example table below.

<div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163014.png" alt=""><figcaption></figcaption></figure></div>



<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163022.png" alt=""><figcaption></figcaption></figure>

<img src="../.gitbook/assets/image.png" alt="" data-size="line"> For the root folder of the company-wide Document Drive, list view permission is granted to all employees by default.

<img src="../.gitbook/assets/image (1).png" alt="" data-size="line"> Permissions must be newly configured for all department folders, such as **1.Regional Team**.

* When a folder is created, it inherits the permissions of the parent folder by default. Therefore, when the **1.Regional Team** folder is created, the root folder's permissions are applied by inheritance by default, granting list view permission to all employees.
* However, for the **1.Regional Team** folder, only the Regional Sales Team should be granted list view, read, write, and delete permissions, so permissions must be newly configured to not inherit the parent folder's permissions.

The steps to newly configure folder permissions are as follows.

1.  In Windows Explorer, select the folder for which you want to set permissions, right-click, and select **Folder Management - Set Permission**.

    <figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163029.png" alt=""><figcaption></figcaption></figure>
2.  &#x20;In the '<Folder> Properties' window, check the **Set Permissions** option, then click the **Add** button.\
    &#x20;     &#x20;

    <div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163036.png" alt=""><figcaption></figcaption></figure></div>
3.  In the 'Select Group(Dept.) or User' window, select the department to grant permissions to from the **Entire List** on the left, then click the **Add >>** button. Next, verify the added department in the **Selected List** on the right, then click the **OK** button at the bottom. \
    &#x20;         &#x20;

    <div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163043.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="success" icon="lightbulb-exclamation-on" %}
If it is difficult to find in the Organization Chart tree, you can also click the search button to search for departments/users.
{% endhint %}

4. In the '<Folder> Properties' window, verify the department added to the **Team/Group or User Names** list, then select permissions in the **Permissions** section at the bottom. In this example, check **Full Control** under the **Allow** column to grant all permissions including list view/read/write/delete. Also, uncheck **Inherit the permissions (from the parent folder)** at the bottom to prevent inheriting the parent folder's permissions. Click **OK** after completing all settings.&#x20;

<div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163050.png" alt=""><figcaption></figcaption></figure></div>

5. Click **Yes** in the window confirming the application to sub-departments to complete the folder permission settings.

<div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163058.png" alt=""><figcaption></figcaption></figure></div>

6. Right-click on the folder and select **Folder Management – Folder Permission Status** to view the configured folder permissions. In the example below, you can see that read, write, delete, list view, and folder creation permissions have been granted to the Regional Sales Team for the **1.Regional Team** folder.       &#x20;

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 170737.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="square-poll-horizontal" %}
Folder Permissions are configured by granting permissions such as list view, read, write, and delete to specific departments or users. For information on Folder Permissions, refer to [**Introduction to Folder Permissions**](https://app.gitbook.com/s/vQ0BiQsGY4PT08D7Nfay/basicmodule/centralfile/undefined-4).
{% endhint %}

{% hint style="warning" icon="square-poll-horizontal" %}
If you designate a **Folder Manager** for the created folder, the Folder Manager can subsequently perform management tasks for that folder, such as creating sub-folders and configuring permissions, on behalf of the Service Administrator. For more details, refer to [**Configuring the Folder Manager**](https://app.gitbook.com/s/vQ0BiQsGY4PT08D7Nfay/basicmodule/undefined-3/undefined-1).
{% endhint %}

#### Setting Folder Permissions in a Multi-Level Structure

When creating department folders in stages following the same structure as the Organization Chart, folder permissions can be designed and configured more precisely. This section explains permission configuration methods using the example of adding sales team folders and a shared sales team folder under the **1.Sales Dept** folder, and creating additional sub-folders within each folder, as shown in the figure below.&#x20;

<div align="left"><figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163113.png" alt=""><figcaption></figcaption></figure></div>



The following table provides examples of the required permissions for each folder under the **1.Sales Dept** folder and summarizes how to grant those permissions.

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 163133.png" alt=""><figcaption></figcaption></figure>

1. For folders marked with <img src="../.gitbook/assets/image (2).png" alt="" data-size="line"> in the table, such as the **1.Sales Dept** folder, permissions must be newly configured.

* When a folder is created, it inherits the permissions of the parent folder by default. Therefore, when the **1.Sales Dept** folder is created, the root folder's permissions are applied by inheritance by default, granting list view permission to all employees.
* However, for the **1.Sales Dept** folder, only the Sales Department should be granted list view and read permissions, so permissions must be newly configured to not inherit the parent folder's permissions.
* For instructions on setting folder permissions, refer to the [**Setting Folder Permissions in a Single-Depth Structure**](undefined-1.md#id-1) section.



2. For folders highlighted in gray in the table, such as **1.Quotations**, no separate permission configuration is needed, and the permissions inherited from the parent folder are applied as-is.

* For the **1.Quotations** folder, team members of the Regional Sales Team must be granted list view, read, write, and delete permissions, the same as the parent folder **1.Regional Team**. Since the required permissions are the same as the parent folder, no separate configuration is needed.
* If no separate permissions are configured for a folder, the changed permissions are automatically inherited even when the parent folder's permissions are updated. For example, after configuring the permissions of the **1.Regional Team** folder as shown in the table, checking the folder permission status of the sub-folder **1.Quotations** shows that list view, read, write, delete, and other permissions have been granted to the Regional Sales Team as **Inherited Permission**, as shown below.

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 170753.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="square-poll-horizontal" %}
Right-click on the folder and select **Folder Management – Folder Permission Status** to view the folder permission configuration status. To view Inherited Permissions, you must check the inherited permission option in the **Permission Type** field.
{% endhint %}
