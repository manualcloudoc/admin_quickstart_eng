# Admin Quick Start Guide – Creating Document Centralization Users and Organization Chart

The administrator must first register all employees in the company as Document Centralization users. Then, referring to the company's Organization Chart as shown in the example below, define the department structure and assign each user to their respective department to complete the Organization Chart.

<figure><img src="../.gitbook/assets/스크린샷 2026-08-12 162830.png" alt=""><figcaption></figcaption></figure>

The created Organization Chart is used as follows:

* Setting access permissions for Department Document Drive folders by department, user, and position in the Organization Chart
* Applying various security policies by department and user unit in the Organization Chart
* Designating Approvers for requests requiring approval, such as Document Export

#### Registering Document Centralization Users and Department Information <a href="#undefined" id="undefined"></a>

To create the Organization Chart for the first time, enter all users, departments, positions, and affiliation information in a data file in the specified format and register them in bulk on the server. For the registration method, refer to [**Registering Organization Chart and Users in Bulk**](https://mcloudoc-manual.gitbook.io/cloudoc-admin-manual/basic/undefined-6).

{% hint style="warning" %}
* You can also use the **Organization Chart Editor** to add users, departments, and positions individually, and assign them to their respective departments. For instructions on using the Organization Chart Editor, refer to [**Introduction to the Organization Chart Editor**](https://mcloudoc-manual.gitbook.io/cloudoc-admin-manual/basic/undefined-7/undefined).
* Adding and registering users is also available from the **User management** menu on the admin webpage.
* In addition, users can be registered and the Organization Chart can be configured through integration with the customer company's DB or AD (Active Directory). However, this feature is not included in the standard scope and requires separate integration development tailored to the customer company's environment.
{% endhint %}



#### Designating Team Document Manager/Team Manager <a href="#undefined-1" id="undefined-1"></a>

After registering the Organization Chart, you must designate a Team Document Manager for each department in the Organization Chart Editor. The Team Document Manager has the authority to approve or reject requests that require security approval, such as Document Export and Copy Document Link, and one of the Team Document Managers can be designated as a Team Manager.

When submitting a request for an action that requires approval, users can select an Approver from among the Team Document Managers/Team Managers of their direct department or parent departments. For example, in the Organization Chart above, the user Hong Gil-dong can select an Approver from among the Team Document Managers/Team Managers of the **국내영업팀, 영업본부, and Our Company**. If no Team Document Manager or Team Manager exists in any department, the action cannot be submitted.

For instructions on designating Team Document Managers, refer to [**Designating Team Manager and Team Document Manager**](https://mcloudoc-manual.gitbook.io/cloudoc-admin-manual/basic/undefined-7/undefined-5).
