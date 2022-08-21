# Create Custom Buttons and Links

## Learning Objectives
After completing this unit, you'll be able to:
- Create custom buttons and links.
- Add them to a page layout.
- Explain the difference between a custom button and a custom link.


## Custom Buttons and Links
Every org has a unique set of business needs. If your users frequently need to access other pages in or outside your org, you can add custom buttons and links directly to object and record detail pages.

Custom buttons and links help you integrate Salesforce data with external URLs, applications, your company’s intranet, or other back-end office systems.

When your users have all the information they need on hand, they can be even more productive with Salesforce.


## What Can Custom Buttons and Links Do?
Custom links can link to an external URL, such as www.google.com, a Visualforce page, or your company’s intranet. Custom buttons can connect users to external applications, such as web pages, and launch custom links.

You can choose the display window properties that determine how the target of a link or button is displayed to your users. Custom links can include Salesforce fields as tokens within the URL. For example, you can include an account name in a URL that searches Yahoo: `http://search.yahoo.com/bin/search?p={!Account_Name}`.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

If you want the button or link to launch a custom page or other code, consider a Visualforce page. If you don’t know how to use Visualforce pages yet, don’t worry. We don’t address them here, but you can learn about them in a different module.

In Lightning Experience, custom buttons and links live on your page layouts and appear in different areas of a Lightning page.

There are three primary types of custom buttons and links that you can create.

- List button—Appears on a related list on an object record page.
- Detail page link—Appears in the Links section of the record details on an object record page.
- Detail page button—Appears in the action menu in the highlights panel of a record page.

We’ll explore all three of these options.


## Create a Custom List Button
You’ve read what they can do, now find out how to create one. For each type, you must define the action that occurs when a user clicks it. First, the custom list button.

A custom list button is a button that you can add to a related list. When you create a list button for an object, you can add that button to that object’s related list when the related list appears on other objects. Because Energy Audits are tied to accounts with a lookup relationship field, an Energy Audits related list automatically appears on account records.

For example, earlier in the module you entered audit information for “GenePoint 5-year review.” When you view the GenePoint account record, then click the Related tab and scroll to the end of the record page, you see an Energy Audits related list displaying that audit.

Maria wants to add a custom button to that Energy Audits related list to let users navigate directly to the Ursa Major Solar energy audit guidelines PDF. She’s already uploaded the PDF as a file, but she needs its URL in order to have the custom button point to it. Here’s how that works.

1. From the App Launcher, find and select the Sales app.
2. Click the **Files** tab. Here, Maria can see the guidelines PDF she uploaded.![Files list view](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/e9bdcea538fd8523fbd8a0b84fecccdb_lex-customization-list-button-1.png)
3. Upload a file of your own so you can follow along with the rest of these steps.
4. Click ![Action dropdown](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/8d48df2da24076f81fe33c1b82647c22_cjgr-1-hsfu-00-bk-0-vcz-89-e-61-rqx.png) for the image you just uploaded and select **Share**.
5. Click the carat next to Who Can Access to expand that section.
6. In the Public Link Sharing area, click **Create Link**. This generates a public URL for the file that you can share with others, or in this case, add as a URL to a custom button or link. In this example, the URL is `https://ursamajorsolar.salesforce.com/sfc/p/R00000008nD1/a/R000000007LK/8Z8auAJBSeSCzqQ8Kv9ofolIWi_jP13oR3LUUYuXc3A`.
7. Click **Copy Link**, then click **Done**.
8. From Setup, click **Object Manager**, then click **Energy Audit**.
9. Click **Buttons, Links, and Actions**, then **New Button or Link**.
10. Name the button `Audit Guidelines`.
11. Select **List Button**.
12. Paste the file URL into the large text box. Use everything after the domain portion of the URL to create the custom link. Using this example, the link points to `/sfc/p/R00000008nD1/a/R000000007LK/8Z8auAJBSeSCzqQ8Kv9ofolIWi_jP13oR3LUUYuXc3A`. ![List button attributes](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/062c5f1c6b9427d537f8d06154bfca75_lex-customization-list-button-2.png)You might be thinking to yourself: “OK, whoa! What’s all that formula-looking stuff? What do I do with that?” That’s a version of Salesforce’s formula editor, and you use it to define the properties of the button or link. For example, if your content source is URL as in this case, this section is where you put the URL you want the button or link to point to. And, you can add merge fields and operators to enhance the behavior of the button or link by including data from Salesforce. For more information on merge fields and operators, check out the Salesforce Help.
13. Click **Save**, then **OK**. The button won’t appear on the Energy Audits related list until Maria adds it. That’s next.
14. Click **Object Manager**, then click **Account**.
15. Click **Page Layouts**, then click **Account Layout**.
16. Scroll all the way down the end of the layout, to the Energy Audits related list.
17. Click the wrench icon to edit it. ![Energy Audits related list](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/d059fcd31515f8e422e19ee6ca9fe9f7_lex-customization-list-button-3.png)
18. Click the plus icon to expand the Buttons section header. ![Related list edit](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/132c07cf234296f07349cdba1282e106_lex-customization-list-button-4.png)
19. Add the Audit Guidelines button to the Selected Buttons list, then click **OK**.
20. Click **Save**.
21. Navigate back to the Sales app, click **Accounts** and select the GenePoint account.
22. Click the **Related** tab, scroll to the bottom, and you see the new Audit Guidelines button on the Energy Audits related list. ![Energy Audits related list with new button](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/b2b06947893043c0cf7f141a43f277d4_lex-customization-list-button-5.png)



## Create a Custom Detail Page Link
Maria, our Ursa Major Solar admin, wants to build on the Energy Audit custom page layout she created for the sales team. She wants to add a custom link that points to the energy cost data from the U.S. Energy Information Administration. This will help the sales reps compare what the customer is paying against the U.S. national average.

Let’s get started.

1. From Setup, click **Object Manager**, then click **Energy Audit**.

2. Click **Buttons, Links, and Actions**, then **New Button or Link**.

3. Name the link `US Average Energy Costs`.

4. Make sure that **Detail Page Link** is selected for the display type, and leave the next two fields as-is. ![Custom detail page link attributes](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/e67c8f3d750950e8de78e87091a757ce_lex-customization-custom-detail-page-link-1.png)Now it’s time to add the URL we want this link to point to.

5. In the formula editor, enter `https://www.eia.gov/analysis/`.

6. Click **Save**, then click **OK**.

   You can use **Quick Save** to save and continue editing. Saving validates the URL you defined if you set the content source to URL. Before you can use your custom buttons and links, add them to an object’s page layout. You can then see and use the button or link on a record detail page. Let’s do that next.

   
7. Click **Page Layouts**, then **Energy Audit Sales Layout**.

8. From the Custom Links category in the palette, drag **US Average Energy Costs** into the Custom Links section of the layout. 
![Add the link to the layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/22f3513a51e700b89d9f448460514db2_lex-customization-custom-detail-page-link-2.png)

9. Click **Save**.
   Let’s go check out the results.

10. From the App Launcher, find and select **Energy Audits**.

11. Open an energy audit record.
    The custom link now lives under the Details tab.![Custom link in the details](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/565d5a3a69a116728891939661168b89_lex-customization-custom-detail-page-link-3.png)



## Create a Custom Detail Page Button
Maria wants to add a custom button to account pages that shows the account’s location on Google Maps.
1. From Setup, click **Object Manager**, then click **Account**.
2. Click **Buttons, Links, and Actions**, then click **New Button or Link**.
3. Name the button `Map Location`.
4. Select **Detail Page Button**.
5. Paste this URL into the formula editor: `http://maps.google.com/maps?q={!Account_BillingStreet}%20{!Account_BillingCity}%20{!Account_BillingState}%20{!Account_BillingPostalCode}` ![Custom detail page button attributes](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/1cfbbe377d927dedc30f1df879594ae2_lex-customization-custom-detail-page-button-1.png)This URL uses merge fields (`{!Account_BillingStreet}`) and passes the field information from the account record that the button is clicked from into the URL.
6. Click **Save**, then click **OK**.
   Now add it to the Account page layout.
7. Click **Page Layouts**, then click **Account Layout**.
8. From the Buttons category in the palette, drag **Map Location** into the Custom Buttons area on the page layout. ![Add the button to the page layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/03ca5c90e46750632a27a62c7489e972_lex-customization-custom-detail-page-button-2.png)
9. Click **Save**. OK! Now let’s test it.
10. From the App Launcher, find and select **Sales**, then click the **Accounts** tab.
11. Open an account record.
    In the highlights panel, not only do you see the fields from the object’s compact layout, but you also see an actions menu. The actions menu is a combination of the standard buttons, custom buttons, and actions from the page layout. (We’ll go over actions in the next unit.)
12. Expand the actions menu, and select **Map Location**. The browser opens a new window or tab that shows you the account’s address in Google Maps. ![Actions menu and the new button](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_buttons_links/images/41178881b7d8171d149be89e9f8b96bd_lex-customization-custom-detail-page-button-3.png)
    Is Map Location not showing up in the actions menu even though you added the custom button to the page layout? This happens sometimes if you override the default settings of the "Salesforce Mobile and Lightning Experience Actions" section of a page layout. To fix it, add any missing buttons to the page layout as actions by dragging them from the "Mobile & Lightning Actions" category in the palette into the "Salesforce Mobile and Lightning Experience Actions" section.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Custom detail page buttons and links can do the same things. Consider where and how you want them to appear on your page, and that can help you decide which type to choose.


## Resources
- [Define Custom Buttons and Links](https://help.salesforce.com/HTViewHelpDoc?id=defining_custom_links.htm&language=en_US)
- [Custom Button and Link Samples](https://help.salesforce.com/HTViewHelpDoc?id=links_useful_custom_buttons.htm&language=en_US)
- [Constructing Effective Custom URL Buttons and Links](https://help.salesforce.com/HTViewHelpDoc?id=custom_links_constructing.htm&language=en_US)
- [Custom Button Considerations](https://help.salesforce.com/HTViewHelpDoc?id=links_considerations.htm&language=en_US)


## Hands-on Challenge
**+500 points**

### GET READY

You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE
Add a Custom Button to a Contact

Ursa Major Solar wants to be able to look at their contacts’ internet footprints. Create a custom button so users can do this right from a contact record.

- Create a custom button for the Contact object:
  - Label: **Google Info**
  - Name: **Google_Info**
  - The custom button opens a link to **https://www.google.com/search?q={!Contact.Name}** (where {!Contact.Name} is the current contact's name)
  - Add the custom button to the Contact Layout page layout