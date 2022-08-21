# Power Up with AppExchange

## Learning Objectives
After completing this unit, you’ll be able to:

- Develop your own AppExchange strategy.
- Install an app from AppExchange.

## What Is AppExchange?
You’re probably comfortable with the idea of app stores. Whether you’re downloading apps on your phone, tablet, computer, or other device, you have to download and install apps to make the most of your technology.

Salesforce is the same way. Earlier, we mentioned the enterprise ecosystem. Salesforce has a community of partners that use the flexibility of the Salesforce platform to build amazing apps and other solutions that anyone can use. These offerings are available (some for free, some at a cost) for installation on AppExchange.

![The AppExchange homepage.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_developer_console/images/784ba8c71bbedfb8828f4745d1705ccc_platform-basics-appex-home-new.png)

## Strategies for Success
D’Angelo’s DreamHouse app is a raging success among the company real estate brokers. But if we’re being realistic, D’Angelo is only one guy. There are only so many hours in the day for him to develop new apps for his colleagues.

Luckily, AppExchange is full of apps D’Angelo can download to help DreamHouse manage everything from payroll to travel approval to integrations with other tools like Evernote and MailChimp.

The possibilities AppExchange offers are exciting, but before you start downloading every app in sight you need to develop a strategy. A solid AppExchange strategy helps ensure that you’re getting the highest value apps without duplicating functionality or investing in something that you don’t need.

Follow these steps to develop a good AppExchange strategy.

1. Identify departments that use or plan to use Salesforce. These are your primary stakeholders.

2. Research what’s available on AppExchange that best meets your stakeholder requirements. Discuss business cases with department heads to determine exact needs. Here are some good questions to ask:

   1. What business problem are you trying to solve?
   2. What are your main pain points right now?
   3. How many users need this app?
   4. What’s your budget?
   5. What’s your timeline?

   These questions help you identify apps that are the best fit for each department or business case.

3. When you find an app that you think meets your needs, download the app in a test environment (like a free Developer Edition or sandbox). Ensure that the app you’re installing doesn’t interfere with any other apps you’ve installed or customizations you’ve made. Sandboxes are copies of your organization in a separate environment. They’re used for development and testing. See [Sandbox Overview](https://help.salesforce.com/articleView?id=create_test_instance.htm&language=en_US).

4. If you’re choosing between multiple apps, take some time to evaluate what you’ve tested. Determine whether there are feature gaps or unwanted functionality. If necessary, invite your stakeholders to demo the apps and provide feedback.

5. You’re ready to go! You’ll install and deploy your app in your production environment. Make sure you keep your users in the loop about what’s changing, and provide training and documentation as necessary.

## Install Your First App
While AppExchange resembles a traditional app store like you can find on your phone or tablet, it’s important to remember that your Salesforce org is a complicated environment. You can’t just install an app because it has a cool logo or a convincing catchphrase.

So what’s the right way to install an app? We’ll show you!

Let’s say you find this great app on [AppExchange](https://appexchange.salesforce.com/) that gives you a fancy set of dashboards for your org.

![The AppExchange Dashboard Pack's AppeExchange page.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_developer_console/images/c2d82e9e2844f3660876d28a78cf8f5a_platform-basics-appex-app.png)

To install the app, click **Get It Now**. This button takes you to the installation wizard that guides you through the steps. Here are two key questions you need to answer during the installation process:

- Where do I install the app, production or sandbox? In general, it’s a best practice to first install apps in a nonproduction environment. Try installing in a sandbox for your production org or in a Developer Edition org. Testing the app first helps you avoid conflicts in production with things like object names.
- Should I give app permissions to admins only, all users, or specific profiles? That depends on who the app is for. If you want to limit access to a particular set of users, plan to modify those user profiles before you install the app.

## Where’d My App Go?
Congratulations! You’ve installed your first app. Now, if only you could find it…

Apps are installed using something called a package. To find the package:

1. From Setup, search and select Installed Packages in the Quick Find box.
2. Click the name of the package you installed. It will be the same name from the AppExchange download page.
3. Click **View Components** to see more information about the package. The Package Details page shows you all the components, including custom fields, custom objects, and Apex classes in the package. This information helps you determine whether you have any conflicts in your own customizations.

## Some Final Thoughts
As you start to explore AppExchange, be sure to check out free apps provided by Salesforce Labs. The great thing about Salesforce Labs apps, other than that they’re free, is that they’re open source. You can customize them as needed and peek under the hood to see how they work. It’s a great way to learn more about how the platform works.

Speaking of learning more, this module has given you a great foundation for diving deeper into the Salesforce platform. Check out the resources below for some potential next steps in your journey. Happy trails!

## Resources
- [AppExchange](https://appexchange.salesforce.com/)
- [Salesforce Admins Blog: Create an AppExchange Strategy](https://admin.salesforce.com/creating-an-appexchange-strategy)

## Quiz

**+100 points**

> **1**- When you're getting started with AppExchange, a best practice is to:

**A.**Install apps of interest right away.

**B.**Request the top 3 apps from each department.

==**C.**Develop a plan, including budget, timing, and key department use cases.==

**D.**Install apps directly into production.

> **2**- When you want to find an app after you install it, what should you enter in the Quick Find box in Setup?**

**A.**Installed Apps

==**B.**Installed Packages==

**C.**Installed Components

**D.**Installations

**E.**Apps

Check the Quiz to Earn 100 Points

Second attempt earns 50 points. Three or more earns 25 points.