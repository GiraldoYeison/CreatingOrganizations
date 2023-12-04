<h1>Creating and configuring an organization<</h1>
<div><b>Creation Date:</b> November 20, 2023</div>
<div><b>Created By:</b> Yeison Giraldo</div>

<div style="height: 24px">&#8203;</div>
<hr />
<div style="height: 24px">&#8203;</div>


<div><h2># Logging as root to your account</h2><p>Remember as best Practice is not to use your root account, in this tutorial we are </p>
</div>

<div><h3>1. The following illustration shows the main steps of the tutorial.</h3>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/6fb3ccfa-742c-4aed-b6de-2cb5a6b8c759/9d7a468d-4c11-4e00-b622-dc8d543f5f58.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="The following illustration shows the main steps of the tutorial." />
</div>

<div><h3>2. Step 1: Create your organization</h3>
<p>In this step, you create an organization with your current AWS account as the management account. You also invite one AWS account to join your organization, and you create a second account as a member account. - we are only creating a second account as member account</p>
</div>

<div><h3>3. Step 2: Create the organizational units</h3>
<p>Next, you create two organizational units (OUs) in your new organization and place the member accounts in those OUs.</p>
</div>

<div><h3>4. Step 3: Create the service control policies</h3>
<p>You can apply restrictions to what actions can be delegated to users and roles in the member accounts by using <a target="_blank" rel="noopener noreferrer nofollow" href="https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html">service control policies (SCPs)</a>. In this step, you create two SCPs and attach them to the OUs in your organization.</p>
</div>

<div><h3>5. Step 4: Testing your organization's policies</h3>
<p>You can sign in as users from each of the test accounts and see the effects that the SCPs have on the accounts.</p><p>None of the steps in this tutorial incurs costs to your AWS bill. AWS Organizations is a free service.</p>
</div>

<div><h3>6. Once you log in to your account search for AWS Organizations</h3>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/7f306254-87bc-415d-8688-82b3d9c3d421/99b332cf-ce40-4161-864d-eae3826db966.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=129&mark-y=189&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0xMDEmaD0yMCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Once you log in to your account search for AWS Organizations" />
</div>

<div><h3>7. AWS Management Console</h3>
<ol><li><p>On the introduction page, choose <strong>Create an organization</strong>.</p></li><li><p>In the confirmation dialog box, choose <strong>Create an organization</strong>.</p><h6>Note</h6><p>By default, the organization is created with all features enabled. You can also create the organization with only <a target="_blank" rel="noopener noreferrer nofollow" href="https://docs.aws.amazon.com/organizations/latest/userguide/orgs_getting-started_concepts.html#feature-set-cb-only">consolidated billing features</a> enabled.</p><p>AWS creates the organization and shows you the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts"><strong>AWS accounts</strong></a> page. If you're on a different page then choose <strong>AWS accounts</strong> in the navigation pane on the left.</p><p>If the account you use has never had its email address verified by AWS, a verification email is automatically sent to the address that is associated with your management account. There might be a delay before you receive the verification email.</p></li><li><p>Verify your email address within 24 hours. For more information, see <a target="_blank" rel="noopener noreferrer nofollow" href="https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_org_create.html#about-email-verification">Email address verification</a>.</p></li></ol><p>You now have an organization with your account as its only member. This is the management account of the organization.</p>
</div>

<div><h3>8. Invite an existing account to join your organization</h3>
<h6>To invite an existing account to join</h6><ol><li><p>Navigate to the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts"><strong>AWS accounts</strong></a> page, and choose <strong>Add an AWS account</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/e9ed5e3f-d65a-4777-ab32-58756edcf368/3dbe73b7-6c1d-461e-9129-881bb132b63b.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=1010&mark-y=99&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0xODImaD0zOCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Invite an existing account to join your organization" />
</div>

<div><h3>9. Invite an existing AWS account</h3>
<ol><li><p>In the box <strong>Email address or account ID of an AWS account to invite</strong> box, enter the email address of the owner of the account that you want to invite, similar to the following: <code>member222@example.com</code>. Alternatively, if you know the AWS account ID number, then you can enter it instead.</p></li><li><p>Type any text that you want into the <strong>Message to include in the invitation email message</strong> box. This text is included in the email that is sent to the owner of the account.</p></li><li><p>Choose <strong>Send invitation</strong>. AWS Organizations sends the invitation to the account owner.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/203e477c-8123-41e8-8a03-f17188bf50b6/c0516eb3-a0d1-425d-8472-6d3e1a36d107.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.4265&fp-y=0.4588&fp-z=1.3819&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=249&mark-y=328&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz03MDMmaD00MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Invite an existing AWS account" />
</div>

<div><h3>10. Create a member account</h3>
<ol><li><p>On the AWS Organizations console, on the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts"><strong>AWS accounts</strong></a> page, choose <strong>Add AWS account</strong>.</p></li><li><p>On the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts/add/create"><strong>Add an AWS account</strong></a> page, choose <strong>Create an AWS account</strong>.</p></li><li><p>For <strong>AWS account name</strong>, enter a name for the account, such as <code>Main Account</code>.</p></li><li><p>For <strong>Email address of the account's root user</strong>, enter the email address of the individual who is to receive communications on behalf of the account. This value must be globally unique. No two accounts can have the same email address. For example, you might use something like <code>mainapp@example.com</code>.</p></li><li><p>For <strong>IAM role name</strong>, you can leave this blank to automatically use the default role name of <code>OrganizationAccountAccessRole</code>, or you can supply your own name. This role enables you to access the new member account when signed in as an IAM user in the management account. For this tutorial, leave it blank to instruct AWS Organizations to create the role with the default name.</p></li><li><p>Choose <strong>Create AWS account</strong>. You might need to wait a short while and refresh the page to see the new account appear on the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts"><strong>AWS accounts</strong></a> page.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/e977c574-082a-42fe-8271-0ab3e6898b3f/c4a788da-76e3-4d24-a95e-6a25d1e5ad20.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Create a member account" />
</div>

<div><h3>11. STEP 2: Create the organizational units</h3>
<p>In the steps in this section, you create organizational units (OUs) and place your member accounts in them. When you're done, your hierarchy looks like the following illustration. The management account remains in the root. One member account is moved to the Production OU, and the other member account is moved to the MainApp OU, which is a child of Production.</p><p><br></p>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/9f937976-e7fd-4981-9c8f-29ad81fd9a7b/16fdc125-d9a4-41c1-adb2-76ef4f65c89b.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="STEP 2: Create the organizational units" />
</div>

<div><h3>12. Note</h3>
<p>In the steps that follow, you interact with objects for which you can choose either the name of the object itself, or the radio button next to the object.</p><ul><li><p>If you choose the name of the object, you open a new page that displays the objects details.</p></li><li><p>If you choose the radio button next to the object, you are identifying that object to be acted upon by another action, such as choosing a menu option.</p></li></ul><p>The steps that follow have you choose the radio button so that you can then act on the associated object by making menu choices.</p>
</div>

<div><h3>13. To Create new O.U.</h3>
<ol><li><p>Choose the check box next to the <strong>Root</strong> container.</p></li><li><p>On the <strong>Children</strong> tab, choose <strong>Actions</strong>, and then under <strong>Organizational unit</strong>, choose <strong>Create new</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/93a6ec69-6719-452d-be7d-e24e8bebecf5/a445c06d-8045-4c35-a761-c3cda2eb3f9f.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=979&mark-y=286&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yMTgmaD0zNCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="To Create new O.U." />
</div>

<div><h3>14. Click on Create organizational unit</h3>
<ol><li><p>On the <strong>Create organizational unit in Root</strong> page, for the <strong>Organizational unit name</strong>, enter <code>Production</code> and then choose <strong>Create organizational unit</strong></p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/ea61d6e5-7cd8-444c-ad08-372d8a1926de/6887a0b5-a235-48b2-82ea-7c91466bf671.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Create organizational unit" />
</div>

<div><h3>15. Move member account to O.U</h3>
<ol><li><p>Return to the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts"><strong>AWS accounts</strong></a> page, and then expand the tree under your <strong>Production</strong> OU by choosing the triangle next to it. This displays the <strong>MainApp</strong> OU as a child of <strong>Production</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/e518b713-daab-4ae9-b1c9-264cdcbb3d18/3a020e14-bd90-41da-980c-29725da9b603.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=380&mark-y=501&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yMSZoPTIxJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Move member account to O.U" />
</div>

<div><h3>16. Select O.U to move member account to</h3>
<ol><li><p>Next to <strong>Memberaccount</strong>, choose the check box (not its name), choose <strong>Actions</strong>, and then under <strong>AWS account</strong>, choose <strong>Move</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/36bb1335-616c-4fe6-92b8-716fd31f3807/46658353-e293-46ed-b914-64410d9f9c23.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=970&mark-y=391&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yMTYmaD0zMyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Select O.U to move member account to" />
</div>

<div><h3>17. Select O.U to move member account to</h3>
<ol><li><p>On the <strong>Move AWS memberaccount </strong> page, choose the triangle next to <strong>Production</strong> to expand it. Next to <strong>Production</strong>, choose the radio button (not its name), and then choose <strong>Move AWS account</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/14be7f3e-92f1-437c-9843-be3420821f39/5e9511db-9188-44db-a96c-569184fa1b8f.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=380&mark-y=557&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yMSZoPTIxJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Select O.U to move member account to" />
</div>

<div><h3>18. Step 3: Create the service control policies</h3>
<h3><strong>Enable the service control policy type for the organization</strong></h3><p>Before you can attach a policy of any type to a root or to any OU within a root, you must enable the policy type for the organization. Policy types aren't enabled by default. The steps in this section show you how to enable the service control policy (SCP) type for your organization.</p>
</div>

<div><h3>19. Enable Policies</h3>
<ol><li><p>Navigate to the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/policies"><strong>Policies</strong></a> page, and then choose <strong>Service control policies</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/f3ba24ea-1859-4305-bbe8-ff8407de8f74/08b1c605-0f94-47f7-bc45-71e40cf8f906.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=121&mark-y=918&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yMzgmaD0xMTMmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Enable Policies" />
</div>

<div><h3>20. Click on Service control policies</h3>
<ol><li><p>On the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/policies/service-control-policy"><strong>Service control policies</strong></a> page, choose <strong>Enable service control policies</strong>.</p><p>A green banner appears to inform you that you can now create SCPs in your organization.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/7f01556b-d07b-4678-a16b-475434f0d428/7dd06694-4d72-49e6-b83c-cee2f8187f51.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=324&mark-y=445&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0xNTUmaD0yNSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Service control policies" />
</div>

<div><h3>21. Step 3: Create the service control policies</h3>
<p>In the steps in this section, you create three <a target="_blank" rel="noopener noreferrer nofollow" href="https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html">service control policies (SCPs)</a> and attach them to the root and to the OUs to restrict what users in the organization's accounts can do. The first SCP prevents anyone in any of the member accounts from creating or modifying any AWS CloudTrail logs that you configure. The management account isn't affected by any SCP, so after you apply the CloudTrail SCP, you must create any logs from the management account.</p>
</div>

<div><h3>22. Enable the service control policy type for the organization</h3>
<p>Before you can attach a policy of any type to a root or to any OU within a root, you must enable the policy type for the organization. Policy types aren't enabled by default. The steps in this section show you how to enable the service control policy (SCP) type for your organization.</p>
</div>

<div><h3>23. Click on Policies</h3>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/d7f002e6-67f6-4427-b348-bc96ca0bb168/9da160cc-94c0-45e6-a9a4-09a66239d0df.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=124&mark-y=935&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yNDMmaD0xMTUmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Policies" />
</div>

<div><h3>24. Click on Service control policies</h3>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/c26f5184-87f1-4a91-9f19-d9d53e764bd2/3fd36c29-c623-4d9d-b4f9-3e124c5a9eab.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=61&mark-y=524&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0yMDImaD0zMyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Service control policies" />
</div>

<div><h3>25. Click on Create policy</h3>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/ef021825-b6b9-4381-9740-54ffff4e01f3/adc58de3-e426-4c76-b429-b59eccc7dca5.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=998&mark-y=236&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0xNzkmaD01MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Create policy" />
</div>

<div><h3>26. Give Policy a Name Block CloudTrail Configuration Actions.</h3>
<ol><li><p>For <strong>Policy name</strong>, enter <code>Block CloudTrail Configuration Actions</code>.</p></li><li><p>In the <strong>Policy</strong> section, in the list of services on the right, select CloudTrail for the service. Then choose the following actions: <strong>AddTags</strong>, <strong>CreateTrail</strong>, <strong>DeleteTrail</strong>, <strong>RemoveTags</strong>, <strong>StartLogging</strong>, <strong>StopLogging</strong>, and <strong>UpdateTrail</strong>.</p></li><li><p>Still in the right pane, choose <strong>Add resource</strong> and specify <strong>CloudTrail</strong> and <strong>All Resources</strong>. Then choose <strong>Add resource</strong>.</p><p>The policy statement on the left should look similar to the following.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/0b1e87e3-b362-4bdf-8f81-f3c88a402c71/b8881777-df13-48c9-8166-3c1820ba7a36.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=1022&mark-y=1337&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xNzMmaD01MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Give Policy a Name Block CloudTrail Configuration Actions." />
</div>

<div><h3>27. 2nd Policy For name, enter Allow List for All Approved Services.</h3>
<p>For name, enter Allow List for All Approved Services.</p><p>Allow the following services</p>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/9ffc4e6e-cf45-43fe-b542-7577c81150ad/1a5fc40d-64b6-41a1-9d7b-f5321e8a3ba2.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="2nd Policy For name, enter Allow List for All Approved Services." />
</div>

<div><h3>28. 3rd create the third policy that denies access to services that can't be used</h3>
<ol><li><p>In the <strong>Policy</strong> section on the left, select <strong>Amazon DynamoDB</strong> for the service. For the action, choose <strong>All actions</strong>.</p></li><li><p>Still in the left pane, choose <strong>Add resource</strong> and specify <strong>DynamoDB</strong> and <strong>All Resources</strong>. Then choose <strong>Add resource</strong>.</p><p>The policy statement on the right updates to look similar to the following.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/04e24dd9-de18-46ac-86f8-0f2b17789a55/d32bccf4-2f25-4a0f-af76-c2ed2e44f9ec.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=1023&mark-y=1343&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xNzYmaD01MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="3rd create the third policy that denies access to services that can&#039;t be used" />
</div>

<div><h3>29. Attach SCP to O.U.</h3>
</div>

<div><h3>30. Click on Root</h3>
<ol><li><p>On the <a target="_blank" rel="noopener noreferrer nofollow" href="https://console.aws.amazon.com/organizations/v2/home/accounts"><strong>AWS accounts</strong></a> page, choose <strong>Root</strong> (its name, not the radio button) to navigate to its details page.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/145476eb-a04e-4acc-9ee9-0f0c5ac695a8/4c7ed24f-2d91-4f6a-9251-20e4cbe10274.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=391&mark-y=408&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz0zOCZoPTMyJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Root" />
</div>

<div><h3>31. Click on Policies</h3>
<ol><li><p>On the <strong>Root</strong> details page, choose the <strong>Policies</strong> tab, and then under <strong>Service Control Policies</strong>, choose <strong>Attach</strong>.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/6f7f4568-7908-40c8-9b75-393132308759/2f5ab1d2-1378-4a78-9596-39a5f819a829.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=470&mark-y=471&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTMlMkNGRjc0NDImdz05NiZoPTYxJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Policies" />
</div>

<div><h3>32. Click on Attach</h3>
<ol><li><p>On the <strong>Attach a service control policy</strong> page, choose the radio button next to the SCP named <code>Block CloudTrail Configuration Actions</code>, and then choose <strong>Attach</strong>. In this tutorial, you attach it to the root so that it affects all member accounts to prevent anyone from altering the way that you configured CloudTrail.</p><p>The <strong>Root</strong> details page, <strong>Policies</strong> tab now shows that two SCPs are attached to the root: the one you just attached and the default <code>FullAWSAccess</code> SCP.</p></li></ol>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/d990e4a2-df0d-4446-80a6-3c4bc2001741/6c05309e-e8b7-469b-b5ec-e58a14274f65.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=1045&mark-y=965&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xMTQmaD00OSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Attach" />
</div>

<div><h3>33. Click on Attach policy</h3>
<img src="https://images.tango.us/workflows/1a8be7b6-ad9e-4357-961a-17ae952b94bd/steps/0721d7cd-6711-4567-8130-1c75a846ed0a/ffc06b08-a1b0-4055-9520-97d59fe83cc3.png?fm=png&crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.5000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=1017&mark-y=593&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xNjUmaD01OCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw" style="border-radius: 8px; border: 1px solid #F4F2F7;" width="600" alt="Click on Attach policy" />
</div>

<div><h3>34. Step 4: Testing your organization's policies</h3>
<p>You now can <a target="_blank" rel="noopener noreferrer nofollow" href="https://docs.aws.amazon.com/signin/latest/userguide/what-is-sign-in.html">sign in</a> as a user in any of the member accounts and try to perform various AWS actions:</p><ul><li><p>If you sign in as a user in the management account, you can perform any operation that is allowed by your IAM permissions policies. The SCPs don't affect any user or role in the management account, no matter which root or OU the account is located in.</p></li><li><p>If you sign in as a user in account 222222222222, you can perform any actions that are allowed by the allow list. AWS Organizations denies any attempt to perform an action in any service that isn't in the allow list. Also, AWS Organizations denies any attempt to perform one of the CloudTrail configuration actions.</p></li><li><p>If you sign in as a user in account 333333333333, you can perform any actions that are allowed by the allow list and not blocked by the deny list. AWS Organizations denies any attempt to perform an action that isn't in the allow list policy and any action that is in the deny list policy. Also, AWS Organizations denies any attempt to perform one of the CloudTrail configuration actions.</p></li></ul>
</div>

<br/>
<hr/>
<div>
<span>Created with </span><a href="https://tango.us?utm_source=magicCopy&utm_medium=magicCopy&utm_campaign=workflow%20export%20links" target='_blank' style='color: #256EFF'>Tango.us
    </a>
</div>
