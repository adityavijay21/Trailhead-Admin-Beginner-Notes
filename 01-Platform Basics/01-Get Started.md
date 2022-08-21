# Get Started with the Salesforce Platform

## Learning Objectives
After completing this unit, you’ll be able to:
- Define the Salesforce platform.
- Describe the DreamHouse scenario.
- Create a Trailhead Playground.
- Explain the difference between no code (declarative) and programmatic development.

## A Quick Introduction to Salesforce
You might think that Salesforce is just a CRM. It stores your customer data, gives you processes to nurture prospective customers, and provides ways to collaborate with people you work with. And it does all those things. But saying that Salesforce is “just a CRM” is like saying a house is just a kitchen. There’s a lot more to it than that.

Salesforce comes with a lot of **standard functionality**, or out-of-the-box products and features that you can use to run your business. Here are some common things businesses want to do with Salesforce and the features we give you that support those activities.

| You need to:                                        | So we give you:                                         |
| :-------------------------------------------------- | :------------------------------------------------------ |
| Sell to prospects and customers                     | Leads and Opportunities to manage sales                 |
| Help customers after the sale                       | Cases and Communities for customer engagement           |
| Work on the go                                      | The customizable Salesforce mobile app                  |
| Collaborate with coworkers, partners, and customers | Slack, Chatter, and Communities to connect your company |
| Market to your audience                             | Marketing Cloud to manage your customer journeys        |

Depending on what your company purchases, you can get these features and more without lifting a finger. But you can almost think of these features as a model house that a real estate agent shows off. You could certainly live there, but it wouldn’t be your home. It wouldn’t have your art on the wall or that unusual coat rack your Aunt Tilda gave you as a housewarming gift.

That’s where the Salesforce platform comes in. With the platform, you can customize and build whatever it is that makes your company unique. And when you have a business application that’s unique to you, everyone is more successful.

## Stories of Salesforce
Throughout Trailhead, you are introduced to a lot of companies and characters that are using Salesforce in different ways. Let’s meet some of the players.

![These four companies appear throughout Trailhead to help you learn about our services.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/7a166c19872b225c62a5b7899e190c71_platform-basics-stories.png)

1. **Cloud Kicks**—This custom sneaker company is making waves in the footwear industry. They use Salesforce to manage sales and help streamline their complicated order creation and fulfillment process.
2. **Ursa Major Solar**—On the cutting edge of renewable energy, Ursa Major Solar needs business software that doesn’t shy away from groundbreaking technology. They use Salesforce to manage sales and customer service nationwide.
3. **Get Cloudy Consulting**—As one of the best cloud consulting firms in the business, Get Cloudy knows CRM. They use Salesforce to manage existing and potential clients, and they’re always looking for new ways to innovate with Salesforce services.
4. **DreamHouse Realty**—Known for their fresh approach to real estate, DreamHouse uses Salesforce to connect their employees and improve the efficiency of home sales.

We’re digging this house theme, so let’s kick off our first module by looking at DreamHouse Realty. We’ll use DreamHouse’s Salesforce implementation to explain some of the fundamental terms, concepts, and capabilities of the Salesforce platform.

Let’s learn a bit more about DreamHouse.

Michelle is the lead real estate broker at DreamHouse. She finds many potential home buyers through DreamHouse’s web and mobile apps. With the apps, customers can browse available homes and make a favorites list of properties that they’re interested in. They can also reach out to Michelle or other brokers directly to set up showings.

![Michelle, the lead broker at DreamHouse.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/623c191edb68e491561694003a8d76a0_platform-basics-michelle.png)

D’Angelo is DreamHouse’s Salesforce administrator. Using the Salesforce platform, he’s building a suite of custom functionality to support Michelle and her team. Michelle can use this custom functionality to edit and view information about the properties she’s selling, as well as keep track of her potential buyers.

![D'Angelo, the Salesforce Admin at DreamHouse.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/86ebec48fc79e1ac764a0d439b767980_platform-basics-dangelo.png)

Remember, Salesforce comes with standard functionality for tracking common sales objects like accounts, contacts, and leads. But DreamHouse is a realty firm, so it has needs specific to its industry and business model. Throughout this module, we work with D’Angelo to see how the Salesforce platform can meet those needs.

## Get to Know Our Terms
Perhaps you noticed a strange word in that last paragraph: objects. **Object** is one of many important terms you’ll learn as you get to know Salesforce.

First, it’s important to understand what a **database** is in the context of Salesforce. When we talk about the database, think of a giant spreadsheet. When you put information into Salesforce, it gets stored in the database so you can access it again later. It’s stored in a very specific way so you’re always accessing the information you need.

Let’s take a look at a page from the DreamHouse app to define some of its important elements and how they relate to the database.

![A labeled property record.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/cc692c3f83b52641f81d56b626616a0b_platform-basics-terms.png)

1. ==An **app** in Salesforce is a set of objects, fields, and other functionality that supports a business process. You can see which app you’re using and switch between apps using the App Launcher ( ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-2-3-3.png)).==
2. ==**Objects** are tables in the Salesforce database that store a particular kind of information. There are **standard objects** like Accounts and Contacts and **custom objects** like the Property object you see in the graphic.==
3. ==**Records** are rows in object database tables. Records are the actual data associated with an object.== Here, the 211 Charles Street property is a record.
4. ==**Fields** are columns in object database tables. Both standard and custom objects have fields.== On our Property object, we have fields like Address and Price.

Another important term that’s hard to capture in a picture is **org**. ==Org is short for organization, and it refers to a specific instance of Salesforce.== The image here is taken from DreamHouse’s org. Your company can have one or multiple orgs.

That’s a lot of new stuff to tackle. If you don’t get it all right away, don’t worry. As you continue to learn about Salesforce, the terminology will start to come naturally.

## Your First Trailhead Playground
A Trailhead Playground (TP) org is a safe environment where you can practice the skills you’re learning before you take them to your real work. TPs come with all the standard app building and customization tools required to test your app development chops. If you’ve ever heard of a Developer Edition (DE) org, a TP is a special type of DE.

When you sign up for Trailhead, we automatically create a TP for you. So if you haven’t signed up yet, now is a great time to do so. If you’re already signed in, scroll to the bottom of this page and click **Launch** to open your TP.

TP orgs are free and you can have up to 10 of them at a time. To create one, go to any hands-on challenge, click the down arrow next to **Launch** and select **Create a Trailhead Playground**. If you hit your max or want to manage your TPs, you can view and delete them from your Trailhead profile. If you ever need your TP’s username and password, you can access them using the instructions [here](https://trailhead.salesforce.com/help?article=Find-the-username-and-password-for-your-Trailhead-Playground).

Go ahead and launch your TP so we can start getting our hands dirty.

## Install the DreamHouse App

To follow along and practice the steps in this module, you need to install the DreamHouse package in your Trailhead Playground. Follow the instructions here to launch a playground and install the package. You also use this package and playground when it’s time to complete the hands-on challenge.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

If Internet Explorer is your browser of choice, it’s time to move to Plan B. Some features of the DreamHouse app aren’t fully supported in Internet Explorer, so switch over to your next favorite browser for the rest of this module.

1. Launch your Trailhead Playground by scrolling to the bottom of this page and clicking **Launch**.
2. From the App Launcher ( ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-2-3-3.png)), find and select **Playground Starter**.
3. If you don’t see the Playground Starter app, copy [this package installation link](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t3h0000043scGAAQ&_ga=2.139026291.1755209910.1657552632-1459833741.1621449068) and check out [Install a Package or App to Complete a Trailhead Challenge](https://trailhead.salesforce.com/help?article=Installing-a-package-or-app-to-complete-a-Trailhead-challenge) on Trailhead Help. Skip the remaining steps.
4. If you see the Playground Starter app, click the **Install a Package** tab.
5. Paste 04t3h0000043scGAAQ into the **Package ID** field and click **Install**.
6. Select **Install for All Users**, then click **Install**.
7. When it prompts you to Approve Third-party access, click **Yes** and click **Continue**. This provides updated information to the map in the Dreamhouse App.
8. When the installation completes, click **Done**.
9. From the App Launcher ( ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-2-3-3.png)), select the Dreamhouse App.

We go through some of the pieces of this app through the module, but feel free to take a look around before you move on.

## Customize the Salesforce Platform
You already know that you can use the Salesforce platform to develop custom objects and functionality specific to your business. What you might not know is that you can do most of this development without ever writing a line of code.

==Developing without code is known as **no-code** (or declarative**) development**. With no-code development, you use forms and drag-and-drop tools to perform powerful customization tasks. The platform also offers **programmatic development**, which uses things like Lightning components. But if you’re not a programmer, you can still build some amazing things on the platform. ==

Let’s start small. Michelle wants a way to quickly indicate whether a potential home buyer is prequalified for a home loan. To make this change, D’Angelo wants to create a prequalified checkbox on the contact object. In Salesforce-speak, we’re adding a custom field to a standard object. Let’s see how he does it.

1. From the gear icon ( ![The gear icon to open Setup.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/02e863126fef084a82dc1f96dea047ff_lex-setup-gear.png)), click **Setup** to launch the setup page. We use Setup a lot, so remember this step!
2. Click the **Object Manager** tab.
3. Click **Contact**.
4. In the Details panel, click **Fields & Relationships**, and then click **New**.
5. A data type indicates what kind of information your field holds. For this field, pick Checkbox and click **Next**.
6. The Field Label is what you see on the Contact page. Enter Prequalified? and click **Next**.
7. Click **Next** again to accept the default field-level security.
8. Check the checkbox to add the new field to all the Contact Page Layouts and then click **Save**.

You just customized your first object. Great job!

Let’s take a look at what we did. From the App Launcher ( ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-3.png)), find and select **Contacts**. Use the arrow ![The list view arrow icon.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/f5f18ad919738dd709152524a40c067b_platform-basics-listview.png) to view All Contacts and click a contact name. Under the Details tab, you can see your new field. Now it’s easier for Michelle and the other brokers to log and retrieve this important piece of client information.

![A contact detail page with the new Prequalified field displaying.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_intro/images/1046bc38cd50545f7bbbb100c6ea59ea_platform-basics-prequalifed.png)

We added that field pretty quickly. But it turns out that we did more than just add a field. At the same time, the platform did a lot of work under the hood. Obviously the new field was added to the user interface. You can also run reports and create dashboards that reference your new field. The field is even ready to go in the Salesforce mobile app. And you didn’t have to do anything except click Next!

That’s the power of the Salesforce platform. In the next unit, we talk about some of the ways you can harness the platform for your business.

## Resources
- ==[Salesforce Term Glossary](https://help.salesforce.com/articleView?id=glossary.htm&language=en_US&type=0)==

## Ready for the Challenge?
If you were following along in the unit, you've successfully completed a "Prequalified?" checkbox. Now, test out what you learned by making a completely new field. This time around, you'll make a currency field rather than a checkbox. Complete the new challenge below to try out what you learned.

## Hands-on Challenge
**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE

Add a custom field to the Contact object

Many homebuyers who work with DreamHouse Realty are prequalified for a home loan. Brokers need to know how much money their clients can borrow so they can show properties in the right price range. Add a Loan Amount field to the Contact object so brokers can record and see this information.

Note: To pass this challenge, you will create a new custom field (in addition to the one you made earlier in this unit, if you were following along).

- Create a field on the **Contact** object
- Field data type: **Currency**
- Field label: **Loan Amount**
- Field name: **Loan_Amount**