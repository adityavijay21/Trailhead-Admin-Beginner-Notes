# Customize Record Details with Page Layouts

## Learning Objectives
After completing this unit, you’ll be able to:
- Create and manage page layouts.
- Use the page layout editor.
- Assign a page layout to a profile.
- Explain how the page layout editor drives record detail content in Lightning Experience.


## Page Layouts
What you see when you log in to Salesforce for the first time is just the start. You can customize and personalize many things on a given object record page using page layouts.

There are two ways to customize a page in Lightning Experience. You can customize a page’s layout, or customize its contents. These are done with separate tools.

Lightning pages are a collection of Lightning components arranged in regions on the page. You can customize the structure of the page and the position of its components with the Lightning App Builder (learn more in the [Lightning App Builder](https://trailhead.salesforce.com/modules/lightning_app_builder) module right here on Trailhead).

You can customize a page’s contents, such as the fields and buttons that appear on the page, by using a different tool called the page layout editor. The page layout editor, also known as page layouts, helps you manage the content of pages in both our Classic UI and in Lightning Experience. The page layout editor is what we’ll be working with in this unit.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Why do we use the dual-UI page layout editor tool to help customize page content in Lightning Experience? Because the Lightning App Builder can't customize buttons, actions, and fields on pages...yet.

The page layout editor lets you:

- Control which fields, lists of related records, and custom links users see
- Customize the order that the fields appear in the page details
- Determine whether fields are visible, read only, or required
- Control which standard and custom buttons appear on records and related lists
- Control which quick actions appear on the page

You’re probably thinking: buttons, lists, record details? What is all this stuff? Let’s take a quick page layout tour by looking at an example contact record, and then we’ll dive in and customize a layout. We’ll talk more about buttons, links, and actions and how to modify them on page layouts in a later unit.

These are the parts of a page that you can customize using page layouts, to create a personalized view for different teams and processes in your org.

- The **Related** tab (1) contains *related lists*, which are lists of other records that are associated with the record you’re viewing. For example, an account can have related products, contacts, opportunities, and other custom records. Related lists make it easy to find and manage related information.![Related List Page](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/f2328b30f470496532ededd584bc0996_admin-intro-related-list.png)
- The **Details** tab (2) shows information about a record. For example, a contact record detail page shows the name, address, owner, account, and other fields that are used to store information about the contact and other related records. To change the content of the fields on a related or detail page, you can click **Edit** (3).![Detail Page](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/8be7e19c8933341e7be5858168e598c7_admin-intro-detail-page.png)

However, that Edit button doesn’t let you configure which fields appear in the record details. Let’s go over that now.



## Customize the Fields in Your Record Details
Customizing the fields on your record pages is easy, and you can do it with just a few clicks. The Enhanced Page Layout Editor is the go-to place for customizing a Lightning Experience record page’s fields and related lists. It’s called “enhanced” because there’s an earlier version of it. We’ll just refer to it as the page layout editor here.

The page layout editor has two basic parts: a palette on the upper portion of the screen (1) and the record’s page layout on the lower portion of the screen (2). The palette contains the basic elements—such as fields, actions, buttons, links, and related lists—that you can add and arrange on your page. You can think of the upper part as the buffet table and the lower part as the plate of food you’re assembling.

Here’s the page layout editor for a lead.![Lead Page Layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/3630372aabded27e959a190555921e86_admin-intro-pl-lead-layout.png)

Maybe you’re thinking, “Hey, what’s that ‘Highlights Panel’ section there? Didn’t you tell us that a compact layout controls the highlights panel on Lightning Experience record pages?” Yes, we did. And that’s still true. This Highlights Panel section in the page layout editor controls the highlights panel on pages in our Classic UI. It’s of no use to us in Lightning Experience.

For now, let’s take a quick tour of the page layout editor by adding and changing a basic field on a lead record.

1. First, we need to find and open the lead page layout.
   1. From Setup, click **Object Manager**.
   2. Click **Lead** to open the object and then click **Page Layouts**.
2. Click **Lead Layout**.
   Now that we’ve opened the lead page layout, let’s make an update. As we all know, fax machines are so last century. So let’s remove that field.
3. Drag the **Fax** field off the page layout and back onto the palette.![Modifying a Page Layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/60da39e1600f7af265c8ddcb8ed901d8_admin-intro-pl-mobile.png)Easy, right? Now, let’s make sure the sales reps don’t leave the Mobile field blank. Let’s make it a required field.
4. Hover over the Mobile field, then click the wrench icon.![Edti Icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/b053c611d65926713937a9d17bf91b60_admin-intro-pl-wrench.png)
5. Click **Required** and then click **OK**.
6. Click **Quick Save** to save your changes without closing the page layout editor.

Nice work! You just removed a field and made another field required and you did it without writing a single line of code.

Wondering what the icons mean to the left of some of the field labels? 

- ![Missing Value in Field icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/1b6a09972a662ce8e5981c84792f2287_required-12.gif)―The field must have a value to save the record, but isn’t required on the page layout itself.
- ![Field Must be Included icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/bd34b7198547fb5baea9402b7a045f2b_alwaysdisplay-12.png)―The field must be included on the page layout because an administrator configured the field as universally required or Salesforce automatically requires the field. Although you can’t remove such fields, you can move them to different locations.
- ![Controlling Field icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/455a6571605ec1392ed7e3de3cf42456_controller.gif)―The field is a controlling field.
- ![Dependent Field icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/10258876582e3ba387040f38a033872f_dependent.gif)―The field is a dependent field.
- ![Read-only icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/95029bc774c577f3d4834415a58540f9_lock-12-2.gif)―The field is read-only.

You can assign page layouts to different user profiles. For example, you can create a customized page layout for managers and another page layout for standard users. To change page layout assignments, click **Page Layouts**, then click **Page Layout Assignment**, and then **Edit Assignment**.


## Create a Page Layout
Maria wants to create an Energy Audit page layout just for her sales team so they can have the necessary field and related list information at their fingertips when they view the Energy Audit records.

When the Energy Audit custom object was created, a system default Energy Audit page layout was created too. Right now, everyone in the org who views an Energy Audit record sees the information from that default layout. Maria is going to create a layout just for the sales people.

Let’s follow along.

1. From Setup, click **Object Manager**.
2. Click **Energy Audit**, then **Page Layouts**.
   You should see the system default Energy Audit layout that we mentioned.
3. Click **New**.
   You have two options at this point. You can create a page layout from scratch, or you can choose an existing page layout to clone. Because Maria wants to build on what’s already there for Energy Audit, she’s going to clone the default layout.
4. Select **Energy Audit Layout**.
5. Name the new layout `Energy Audit Sales Layout`.
6. Click **Save**.
7. Scroll down to the Energy Audit Detail section.
   Here’s a comparison of the page layout field details and the Energy Audit fields with the default configuration.![Page layout versus Details section](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/cc11404aafda46ce07534a52de230a97_lex-customization-page-layout-ple-vs-lex-1.png) That right-hand column is almost empty, and the fields could be in a better order. Let’s fix that.
8. Move Audit Notes and Type of Installation to the right column, above Owner.
9. Move Account below Energy Audit Name. ![Customized fields](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/649a3c9352237151aaccb8e459f961b0_lex-customization-page-layout-ple-fields.png)
10. Click **Quick Save**.
    Nice! But there’s more to do. Because Energy Audit is a custom object, it doesn’t have any related lists...yet. Let’s add one.
11. Scroll down to the Related Lists section.
12. In the palette, click **Related Lists**, and drag the **Files** element down to the Related Lists section.
    With the Files related list, Ursa Major Solar sales reps can add files to a record and see a list of files associated with the record.
13. Click **Quick Save** again, then click **Yes**.
    We’re done with the page layout for now, but no one can see it. Time to assign it to profiles.



## Assign a Page Layout to Profiles
Maria wants Ursa Major Solar’s salespeople to see this new page layout. She’s going to assign it to her sales team’s user profile so when they view Energy Audit records, they’ll see the revised view of the fields and the new related list. Let’s get started.

1. If you’re not already in the Energy Audit object, from Setup, click **Object Manager** | **Energy Audit**.

2. Click **Page Layouts**, then **Page Layout Assignment**. You can see the list of profiles and the page layout assigned to each one.

3. Click **Edit Assignment**.

4. Select the **Custom: Sales Profile** row.

5. From the Page Layout To Use field, select **Energy Audit Sales Layout**.

6. Select the **System Administrator** row. Normally, Maria would select only the Custom: Sales Profile row, but since you’re logged in as a System Administrator, we select that too so that you can check out how the new page layout looks.

7. From the Page Layout To Use field, select **Energy Audit Sales Layout**, then click **Save**. Let’s go see the results!

8. From the App Launcher, find and select

    

   Energy Audits

   , then open an audit record. Look at the Details tab. It’s more condensed and efficient now.

   | Before                                                       | After                                                        |
   | :----------------------------------------------------------- | :----------------------------------------------------------- |
   | ![Details section from the default layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/ebe86e4479453a4e825ac232756d699c_lex-customization-page-layout-sample-lex-1.png) | ![Details section from the new layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_page_layouts/images/e5b47633d0c3811a2382091772a686d7_lex-customization-page-layout-sample-lex-2.png) |

   And, if you click the Related tab, you see the Files related list there now, just waiting for someone to upload something.

Great job! Now that you’re more familiar with page layouts and the page layout editor, you can start creating layouts that give your users just what they need. By arranging tools and fields in logical sections, you can make it even easier for your users to store and manage the data that’s important to your business.



## Resources
- [User Interface Elements for the Enhanced Page Layout Editor](https://help.salesforce.com/HTViewHelpDoc?id=customize_layoutcustomize_pd_elements.htm&language=en_US)
- [Customize Search Layouts to Show Results Users Want](https://help.salesforce.com/s/articleView?id=sf.customizing_search_layouts.htm)
- [Page Layouts in Lightning Experience](https://help.salesforce.com/articleView?id=layouts_in_lex.htm&language=en_US)

## Quiz

**+100 points**

> **1** - With a page layout, you can control:

**A.**Whether a user sees related or details pages

**B.**The fields that display in the highlight panel

==**C.**Which fields, lists, links, and buttons a user sees on related, details, and edit pages==

**D.**The size of the margins of a page

**E.**All of the above

> **2** - When you modify page layouts, you can:

**A.**Change whether a field is required

**B.**Change the order of the fields on the page

**C.**Assign custom page layouts to different user profiles

**D.**Arrange fields in logical sections

==**E.**All of the above==

> **3** - Where do the fields and sections from a page layout appear when you view a Lightning record page?**

**A.**In the Highlights panel

==**B.**Under the Details tab==

**C.**Under the Related tab

**D.**In hover text when you mouseover the record name

Check the Quiz to Earn 100 Points

Second attempt earns 50 points. Three or more earns 25 points.