# Configuring an Active Directory Home Lab

## Objective
This hands-on project allowed me to explore and manage Active Directory objects using the "Active Directory Users and Computers" tool. I created and managed Organizational Units (OU), users, groups, and computer objects, gaining practical experience in Active Directory administration. My main goal of this at-home lab was to become comfortable in the AD environment. I used my university's virtualized environment to do so. I skipped configuring the virtualized environment to reduce the length of this project.




### Skills Learned
- Advanced understanding of Active directory environment.
- Managed OUs, users and groups gaining practical experience in AD administration
- Development of critical thinking and problem-solving skills in cybersecurity/IT.


## Steps
drag & drop screenshots here or use imgur and reference them using imgsrc

Every screenshot should have some text explaining what the screenshot is about.


My first step in this project was creating an out-marketing group within AD. To do so I started by navigating to the "Active Directory users and computers" under the "tools" tab.

![temp](https://github.com/user-attachments/assets/bd94433b-55fc-435c-8a86-b4992ac1783e)


Step 2: Created the 'Marketing' Organizational Unit (OU)
I right-clicked the domain and selected the option to create a new Organizational Unit (OU) named "Marketing," following the steps illustrated in the reference image below.

![temp2](https://github.com/user-attachments/assets/e45b99a3-cd1b-4a90-b6b9-0559e24f9d4c)

![temp3](https://github.com/user-attachments/assets/4f6998cc-a5f3-4919-8525-b56b391a57a8)


Step 3: Created Groups within the 'Marketing' OU
After creating the 'Marketing' OU, I created the necessary groups by right-clicking on the domain, navigating to New, and selecting Group.

![temp4](https://github.com/user-attachments/assets/da92d1d4-303d-47e2-9504-42d0b14e0a56)

Step 4: Named the First Group 'Marketing-g'
In the text box, I named the first group "Marketing-g" to align with the naming convention for the 'Marketing' OU.

![temp5](https://github.com/user-attachments/assets/f50e6f25-6efb-4757-9bcc-334f9b694e4c)

Step 5: Created the 'Marketing-U' Group
I repeated the same steps to create an additional group named "Marketing-U," designating it as a Universal group.

![temp6](https://github.com/user-attachments/assets/37cc1621-0e69-425a-adba-744241e71579)

Step 6: Created Test Users for Each Security Group
I proceeded to create test users within each security group by right-clicking the Users folder and following the steps shown in the reference image below.

![temp7](https://github.com/user-attachments/assets/d73ac1e9-e9e2-43e7-8a3c-1eede8fa2aac)

Step 7: Established a Consistent User Login Format
To maintain consistency across the virtual environment for the fictional company, I standardized user logins by adopting the format: firstname.lastname.

![temp8](https://github.com/user-attachments/assets/cc5f0184-f1a4-4e05-9c28-740753f6142c)

Step 8: Enforced Password Security Policies
During user creation, I ensured the "User must change password at next login" option was checked to enforce unique passwords for each user. Additionally, I left the "Password never expires" option unchecked to implement stricter password policies in the future.

![temp9](https://github.com/user-attachments/assets/e946c73e-11a9-47e3-a18a-7a461b1587eb)

Step 9: Added Users to the 'Marketing-g' Group
To assign users to the Marketing-g group, I right-clicked the user within the Users folder and selected "Add to a group." This tab also contains other useful tools, such as the "Reset Password" option for user management.

![temp10](https://github.com/user-attachments/assets/9d32d15f-c251-4eee-8fde-dd9ad9bb6553)


Step 10: Assigned Users to 'Marketing-g' Group
I typed in "Marketing-g", the group created earlier, and clicked "Check Names" to verify the group name and ensure there were no typos before finalizing the addition.

![temp11](https://github.com/user-attachments/assets/921fd943-c582-4e92-b39b-81c1ad91efc2)

Step 11: Created a Group Policy Object (GPO) for Security Policies
To enforce password policies and disable the command prompt for enhanced security, I created a Group Policy Object (GPO). I started by navigating to the Group Policy Management tab under Tools.
![temp12](https://github.com/user-attachments/assets/27743b1f-7d51-47cf-afc9-c486939b26e1)

Step 12: Linked the GPO to the 'Marketing' OU
I expanded the forest domainx.com, then right-clicked on the previously created Marketing OU to create and link the GPO within this domain. This allowed the security policies to apply specifically to the 'Marketing' organizational unit.

![temp13](https://github.com/user-attachments/assets/dcc97fff-a31e-4d3a-8684-0e3ac687e90d)

Step 13: Configured Password Policies
Within the GPO settings, I navigated to the Password Policy tab. Here, I set the Maximum Password Age to 30 days and enforced complex password requirements to enhance security across the domain.

![temp14](https://github.com/user-attachments/assets/d0eef73a-c67a-4de3-a4dc-5cc809f94a70)
![temp15](https://github.com/user-attachments/assets/ea54d2fe-306b-4630-950d-6a89d0dcc8f6)

Step 14: Disabled Command Prompt for Basic Users
As a final security measure, I disabled the Command Prompt for basic users within the Marketing group. Since marketing users have no need for this tool, unlike the IT team, this restriction enhances security by limiting access to advanced system commands.

![temp16](https://github.com/user-attachments/assets/36794120-f758-4a47-8a59-d0ebd2e86916)













