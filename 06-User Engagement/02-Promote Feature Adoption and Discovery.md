# Promote Feature Adoption and Discovery


## Learning Objectives
After completing this unit, you’ll be able to:
- Decide when to use in-app guidance.
- Describe the three types of prompts: floating, targeted, and docked.
- Create prompts and walkthroughs.


## Choosing the Right Subject
Before we get into how to add prompts and walkthroughs, let’s talk a little more about why you add one or the other. They're perfect for the feature discovery and adoption scenarios, such as:

- **New feature is enabled or available**: Experienced users appreciate enhancements to features they use often, and like to be the first to know about new features, as long as the information is helpful and relevant.
- **User isn't taking advantage of a valuable feature**: Sometimes your users aren't using your application to its full potential. To help them follow best practices and take advantage of beneficial features, offer tips, guidance, and instructions focused on saving time and increasing productivity.

How do you choose the right subject for your prompt or walkthrough?

| Good Feature Candidates                                      | Features to Avoid                                            |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| Features that are easy to learn and start using right awayFeatures that are available to users without setup or personalization | Features that are highly complex with hard-to-remember workflowsFeatures that have a steep learning curveFeatures that can be heavily personalized by users |

Now that we talked about the goal and purpose of prompts and walkthroughs, let’s chat about the audience. Although every company and user is unique, remember that generally, users:

- Know the basics, and don’t want their workflow interrupted without good reason
- Want actionable, relevant information about: new possibilities, updates to features they use often, and new features that could increase productivity
- Don’t want to be sold to, unless an offering is clearly tailored to their needs

So, unless you want your prompt to be closed before it’s read, carefully select a subject that speaks to your users.

We have our purpose and audience in mind, so let’s next talk about the difference between prompts and walkthroughs.

## Choosing the Right Type of In-App Guidance
A prompt is a single, small pop-up window that directs users’ attention to a feature, update, or call to action. The user notices the prompt, ingests the information or takes action, and moves on with their day.

A walkthrough is a series of connected prompts that provides a step-by-step guided experience across a single or multiple pages for in-context learning. Walkthroughs do ask more of the user’s time. However, the walkthrough’s unique hands-on learning encourages users to take the time to complete all steps. The whole is definitely more than the sum of its parts.

As you may imagine, walkthroughs aren’t only great for feature discovery and adoption. Think about walkthroughs as a way to:

- Onboard new hires to their workspace.
- Highlight a series of key but related features.
- Provide a navigational or feature overview.
- Guide users through a multi-step procedure.

For feature adoption and discovery, we recommend using a single prompt for a short message. Use a walkthrough when you want to explain a series of connected features or to guide users through some action related to the feature itself.

## Choosing the Right Type of Prompt
Floating prompts are a nonintrusive way to nudge users toward a feature or opportunity. There’s no extra fluff here. Just a short and sweet message, an optional image, and a call to action in the form of a button that opens a URL of your choice. You can spruce up your message using the rich text editor or leave it plain and simple. Floating prompts are also ideal for most steps of a walkthrough. You can place a floating prompt in one of nine positions on a page:
- Top left
- Top center
- Top right
- Middle left
- Middle center
- Middle right
- Bottom left
- Bottom center
- Bottom right

![Floating prompt wireframe](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/3fb29c5c0122631f41686fad8b1a15ff_wireframe-floating-prompt.png)*Floating prompt* Targeted prompts have all of the same benefits as a floating prompt without being confined to nine placement positions. Connect a targeted prompt to a specific page element to show your users exactly what you’re referring to.

![Targeted prompt wireframe](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/6af2a980165f2f069733a7f3bee19d1a_wireframe-targeted-prompt.png)*Targeted prompt* 

Docked prompts are great when users need to refer to content while exploring a feature on their own. Unlike the floating and targeted prompts, the docked prompt stays in place while the user navigates through the app. Use a docked prompt for content that you want to remain on screen, such as step-by-step instructions or an image or short video that users can follow while learning how to complete a task in the app. Consider using a docked prompt to display next steps or takeaways in the last step of a walkthrough.

![Docked prompt wireframe](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/e68a71a31624d0eb5a66005dd433bfcb_dockedprompt.png)*Docked prompt* 

| Choose a floating or targeted prompt when...                 | Choose a docked prompt when...                               |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| Your goal is to drive readers to a resource, such as a training PDF or website.Your goal is to have readers acknowledge information without specifically completing an action.Your message is short (approximately one sentence). | You want to include short, step-by-step instructions that the user can consult while they work.You want to embed a video into the docked prompt.Your message is longer than one sentence. |

## Examples of Prompts
Here are some examples of the different types of prompts. If you want some other examples of prompts, consider installing the [In-App Guidance: Boost Sales User Productivity in Lightning Experience](https://sfdc.co/InAppGuidanceTH) or [In-App Guidance: Boost Service User Productivity in Lightning Experience](https://sfdc.co/SvcInAppGuidanceTH) managed package from Salesforce. It’s a great starting point for building your own library of prompts. To install this package, your org must already have the Sales or Service Console app installed.

![Floating prompt example](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/a670e44f16790b7af938875abd65e6cc_customhelp-prompts-feature.png)

Suppose you want to introduce users to the new layout for the account record detail page. You add a header that indicates the change is important. You give it an engaging title (*Do more with the new account view*). And you embed a helpful video and highlight the main updates, including that Path and key fields are displayed at the top of the record for quick reference.

In a docked prompt, your message would look like this.

![A prompt titled Important Changes has an embedded video about managing accounts and contacts and bullets that highlight key details of the new account view](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/32448b4474088ad0e7816c97f3c0e27c_customhelp-prompts-configchange.png)



## Want to Get Hands-on with In-App Guidance?
We don’t have any hands-on challenges in this module, but if you want to follow along and practice the steps, you need to install the Sales or Service version of the In-App Guidance: Boost User Productivity in Lightning Experience package into your Trailhead Playground. To launch your playground and install the package, follow these instructions.

First, launch your Trailhead Playground.

1. Make sure you're logged in to Trailhead.
2. Then click your user avatar in the upper-right corner of this page, and select **Hands-on Orgs** from the dropdown.
3. Then click the username of your org to launch it.

Next, get your username and password.

1. In your playground, click ![Setup](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/02e863126fef084a82dc1f96dea047ff_lex-setup-gear-4.png) and select **Setup**.
2. Enter **Users** in the Quick Find box, then select **Users**.
3. Check the box next to your name. Make note of your username.
4. Click **Reset Password(s)** and then **OK**. This step sends an email to the address associated with your username. If you don’t see the email, check your spam folder.
5. Click the link in the email.
6. Enter a new password and confirm it.

If you’re having trouble finding your username and resetting your password, see [this article](https://trailhead.salesforce.com/help?article=Find-the-username-and-password-for-your-Trailhead-Playground).

Now you can install the package.

1. In Chrome, open an incognito browser window.
2. Install one of these packages.
   - For prompts for the Sales app, select and copy this link: https://sfdc.co/InAppGuidanceTH. To install this package, your org must already have the Sales app installed.
   - For prompts for the Service app, select and copy this link: https://sfdc.co/SvcInAppGuidanceTH. To install this package, your org must already have the Service Console app installed. 
   - For walkthroughs, select and copy: https://appexchange.salesforce.com/appxListingDetail?listingId=a0N4V00000DYB7bUAH.
3. Click **Get It Now**.
4. On the Salesforce login screen that appears, enter the username and password for your Trailhead Playground, then click **Log In**.
5. Select **Install in Production**.
6. Agree to the terms and click **Confirm and Install**.
7. On the login screen that appears, log in again with your Trailhead Playground credentials.
8. Select **Install for All Users**, then click **Install**.
9. After the installation is complete, click **Done**.

If you have trouble installing the package, see the Install Apps and Packages in Your Trailhead Playground unit of the [Trailhead Playground Management](https://trailhead.salesforce.com/content/learn/modules/trailhead_playground_management) module.

The In-App Guidance: Boost User Productivity in Lightning Experience package that you just installed comes with its own installation and considerations guide.

Let’s take a look at the new prompts you just installed.

1. Click ![Setup](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/02e863126fef084a82dc1f96dea047ff_lex-setup-gear-2-2-2-2-2-2-2-2-2-2-2-2.png) and select **Setup**.
2. In Quick Find, enter in-app, and then select **In-App Guidance**. You should see the prompts installed from the package listed on the setup page.
3. From the row-level action dropdown menu, select **Preview**. A new tab opens allowing you to see how the prompt appears to users.

If these prompts don't precisely meet your needs, you can create your own prompts or walkthroughs.

## Add a Prompt or Walkthrough
Watch this video to see how to use the In-App Guidance Builder and setup page. See the Resources section for more videos about creating prompts and walkthroughs.

To create your own prompts and walkthroughs, follow these steps.

1. Click ![Setup](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/02e863126fef084a82dc1f96dea047ff_lex-setup-gear-2-2-2-2-2-2-2-2-2-2-2-2.png) and select **Setup**.
2. In Quick Find, enter in-app, and then select **In-App Guidance**.
3. Click **Add**. The In-App Guidance Builder opens in a new tab.
4. In the builder, navigate to the page where you want to add the prompt or walkthrough and click **Add**. A sidebar opens on the right side for you to start authoring.
5. Specify if you want a single prompt or a walkthrough and the type, location, and position of the prompt. Then, write the content.
6. To specify the title, body, and button text, select **Next**. You can also include an image, or for docked prompts, embed a video.
7. Click Save. A window opens for additional settings. You can access these settings again by clicking ![Setup](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/user-engagement/promote-feature-adoption-and-discovery/images/529ff46f37f22e7b044954b1bb0df0bc_9-d-4004-b-6-8409-4461-9-c-06-d-97-c-94-be-7491.jpg) in the builder header while editing a prompt or walkthrough.
8. Specify an action button or link, schedule, profile, permissions, active status, and name.
9. Save your changes.
10. When you’re satisfied, click **Done**.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Although you can create custom walkthroughs and install walkthrough packages as an admin, you’ll need to subscribe to myTrailhead to show more than three custom walkthroughs to users at a time. See In-App Guidance in Lightning Experience (in the Resources section) for documentation about walkthroughs.

When you have a lineup of great prompts and walkthroughs, it’s important to monitor user engagement to see if your content is engaging users. Salesforce has made it easy with prebuilt metrics for prompts.

When a prompt is active, view usage metrics on the In-App Guidance Setup page. Views represent the total number of unique users who have seen the prompt. Completes represent the percentage of viewers who have clicked the action button.

Set up a custom report type using the Prompt Actions object. Add the Step Number, Last Display Date, Last Result (look for the Error valid value), Name, and User: Full Name fields as columns in the report. See [Monitor In-App Guidance in Lightning Experience](https://help.salesforce.com/s/articleView?id=sf.customhelp_lex_prompt_monitor.htm) in the Resources for a list of all available fields and links to topics about creating custom reports.

You can download a Salesforce Labs package of pre-built, customizable reports and dashboards. Visit the Salesforce AppExchange to install the free packages for [prompts](https://appexchange.salesforce.com/appxListingDetail?listingId=a0N4V00000G13VjUAJ) and [walkthroughs](https://appexchange.salesforce.com/appxListingDetail?listingId=a0N4V00000G13VoUAJ). Find more information about the package on the AppExchange listing pages, including user guides.

Then start asking questions to identify trends. Did you get more views or clicks on docked, floating, or targeted prompts? Did you get more action button clicks with a certain button label or title? Did longer content get fewer button clicks? Was there a drop-off in engagement during the run of the prompt? Did walkthroughs with more than five steps have a greater drop-off rate than shorter walkthroughs?

It may be difficult to identify exact correlations between behavior and retention, but reviewing metrics helps you fine-tune your location, position, content, and frequency settings.

Keep it going! Prompts and walkthroughs are pretty easy (and fun) to create. You might want to keep making more of them. However, they're only one part of user engagement. In the next unit, you learn about the troubleshooting scenario and the Help Menu.


## Resources
- *Salesforce Help: [Create a Custom Report Type](https://help.salesforce.com/s/articleView?id=sf.reports_defining_report_types.htm&type=5)
- *Salesforce Help*: [In-App Guidance in Lightning Experience](https://help.salesforce.com/articleView?id=customhelp_lexguid.htm&language=en_US)
- *Salesforce Help*: [Monitor In-App Guidance in Lightning Experience](https://help.salesforce.com/articleView?id=customhelp_lex_prompt_monitor.htm)
- *Salesforce Help*: [PromptAction](https://developer.salesforce.com/docs/atlas.en-us.224.0.object_reference.meta/api/sforce_api_objects_promptaction.htm)
- *Video*: [Create a Prompt](https://salesforce.vidyard.com/watch/mfpLNa4prnDNuHS5zJm5wg?)
- *Video*: [Create a Walkthrough](https://salesforce.vidyard.com/watch/hXu7Vomp2bgPc5RSM1U6n3?)

## Quiz
**+100 points**

> **1** - Why would you add prompts?

**A.**A new feature is enabled.

**B.**Users aren't taking advantage of a valuable feature.

**C.**Users frequently leave tasks incomplete.

==**D. A and B==

**E.**B and C

> **2** - What are the benefits of a docked prompt?

==**A. It stays put while the user navigates around.==

**B.**It has a Dismiss button.

**C.**It can display embedded gif images.

**D.**Its prompt isn't intrusive.

**E.**You can place it in one of six positions on the page.

Check the Quiz to Earn 100 Points

Second attempt earns 50 points. Three or more earns 25 points.