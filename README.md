# SIEM-Visualization-Example-3-Successful-RDP-Logon-Related-To-Service-Accounts
SIEM Visualization Example 3: Successful RDP Logon Related To Service Accounts
In the SIEM visualization lab, I performed several key steps to create a targeted visualization for monitoring unusual RDP logon events associated with service accounts. Here are the steps outlined in a numbered format:

Accessing the Visualization Tool:

I logged into Kibana using the provided IP address and accessed the pre-configured dashboard.
Initiating Visualization Creation:

I clicked on the "Create visualization" button to start configuring a new visualization tailored to the specific security needs.
Configuring Data Filters:

I applied filters to isolate successful RDP logon events (Event ID 4624) specifically involving service accounts. This was done by filtering for RemoteInteractive logons and user names beginning with "svc-".
Setting Data Source and Verification:

I specified "windows*" in the "Index pattern" field to focus on Windows event logs and used the search functionality to verify the presence of the user.name.keyword field, ensuring the data's relevance and accuracy.
Selecting Visualization Type:

I chose the "Table" type from the available visualization options, which best suited the data presentation requirements for this scenario.
Configuring Table Columns:

I configured the table rows to include essential details such as the service account name, the host machine name where the logon occurred, and the IP address of the initiating machine.
Setting Metrics:

I set up metrics to count the number of occurrences of the filtered events, allowing for quantitative analysis of the data.
Finalizing the Visualization:

I completed the configuration by adding an additional column to display the frequency of the logon events, which helps in identifying and assessing the scope of any security issues.
Saving and Integrating the Visualization:

![Screenshot 2024-07-30 at 10 19 31 AM](https://github.com/user-attachments/assets/bbd5e54a-866f-4bc1-8cfa-90ad264476fa)

I saved the new visualization and returned to the dashboard to integrate it, enabling ongoing monitoring and quick access to the visualization for regular security assessments.
These steps provided a structured approach to using SIEM tools for specific security monitoring tasks, enhancing my ability to address potential security vulnerabilities associated with service account usage in RDP sessions.
