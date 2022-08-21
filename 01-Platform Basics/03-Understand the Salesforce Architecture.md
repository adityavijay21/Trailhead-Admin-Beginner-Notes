# Understand the Salesforce Architecture

## Learning Objectives
After completing this unit, you’ll be able to:

- Define key terms related to the Salesforce architecture.
- Find information related to trust.
- Explain at least one use case for Salesforce APIs.

## What Is the Salesforce Architecture?
By now you know that you can use Salesforce to deliver a highly customized experience to your customers, employees, and partners. You can do it without writing much (or any) code, and you can do it fast.

What’s so special about Salesforce? It all starts with our architecture.

Before you close out this window in a frantic attempt to avoid learning about what seems like a really boring subject, sit tight. Learning about Salesforce architecture is quite interesting, and understanding it makes working with the platform a whole lot easier.

When you think about the Salesforce architecture, imagine a series of layers that sit on top of each other. Sometimes it helps to think of it as a cake because cake is delicious, and it makes everything better.

![A diagram outlining Salesforce architecture.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_understanding_arch/images/a1b2bb1adfd5c5951a958fb019d4fbd2_platform-basics-arch.png)

There’s a lot to unpack here, but let’s focus on the most important points.
- Salesforce is a cloud company. Everything we offer resides in the trusted, multitenant cloud.
- The Salesforce platform is the foundation of our services. It’s powered by metadata and made up of different parts, like data services, artificial intelligence, and robust APIs for development.
- All our apps sit on top of the platform. Our prebuilt offerings like Sales Cloud and Marketing Cloud, along with apps you build using the platform, have consistent, powerful functionality.
- Everything is integrated. Our platform technologies like predictive analytics and the development framework are built into everything we offer and everything you build.

There are few terms in here that are extra important for you to understand: trust, multitenancy, metadata, and the API.

## Why Trust the Cloud?
At Salesforce, **trust** is our top priority. Not only are you keeping your sensitive data in your org, you’re also building functionality vital to your company’s success on our platform. Our responsibility to keep your data and functionality safe is not something we take lightly, which is why we’re always transparent about our services.

Our trust site, ==[trust.salesforce.com](https://trust.salesforce.com/en/), is a vital resource. You can use it to view performance data and get more information about how we secure your data. It also shows you any planned maintenance we’ll be performing that might impact your access to Salesforce.==

## Sharing Is Caring in the Multitenant Cloud
So far, we’ve been talking a lot about houses. But really, Salesforce is set up more like an apartment building. Your company has its own space in the cloud, but you have all kinds of neighbors, from mom-and-pop shops to multinational corporations.

![An apartment building with dedicated space but shared resources.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_understanding_arch/images/4f32f70d1ea71f7f0aedab004cafaf62_platform-basics-multitenant.png)

This idea is **multitenancy**. ==Multitenancy== is a great word for making you sound smart at dinner parties, but really all ==it means is that you’re sharing resources==. Salesforce provides a core set of services to all our customers in the multitenant cloud. No matter the size of your business, you get access to the same computing power, data storage, and core features.

Trust and multitenancy go hand in hand. Despite the fact that you’re sharing space with other companies, you can trust Salesforce to keep your data secure. You can also trust that you’re getting the latest and greatest features with automatic, seamless upgrades three times a year. Since Salesforce is a cloud service, you never have to install new features or worry about your hardware. All this is possible because of multitenancy.

## The Magic of Metadata
To put it simply, ==**metadata** is data about data.== Wait. That’s not simple at all. When we say data about data, we’re really talking about the structure of your Salesforce org.

Let’s think about an object like Property. When our friends at DreamHouse use Salesforce, they input and view data about properties. For example, a property can be located in Boston, cost $500,000, and have 3 bedrooms.

Now, imagine you stripped away all that specific data. What are you left with? You are left with the Property object along with all its fields, like address, price, and number of bedrooms. You can also have page layouts, security settings, and any other customizations you’ve made.

All of these standard and custom configurations, functionality, and code in your org are metadata. Part of the reason you can move so fast on the platform is that Salesforce knows how to store and serve you that metadata immediately after you create it.

## All About That API
Fundamentally, ==**APIs** allow different pieces of software to connect to each other and exchange information==.

If that sounds kind of abstract, take a quick look at the computer you’re working on right now. You can probably find a series of ports of various shapes and sizes that support different kinds of connections. These are like the hardware version of APIs. You don’t have to know how the USB port works. All you have to understand is that when you plug your phone into a USB port, it passes information to your computer.

APIs are similar. Without knowing the details, you can connect your apps with other apps or software systems. The underlying technology takes care of the specifics of how information passes throughout the system.

So what does this have to do with Salesforce?

Earlier, we talked about the database. When you add a custom object or field, the platform automatically creates an API name that serves as an access point between your org and the database. Salesforce uses that API name to retrieve the metadata and data you’re looking for.

For example, we can use a contact’s Name field in a bunch of places, like the Salesforce mobile app, a custom page, or even an email template. That’s all possible because of the API name.

![An email template in Salesforce using the API name of a contact and property.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/starting_force_com/starting_understanding_arch/images/4f0900e54e0dd0cca78bfd71956dc715_platform-basics-email.png)

The core of the API’s power is that all of your data and metadata is API enabled. This might not seem like a big deal right now, but the API gives Salesforce a huge amount of flexibility. It lets you move beyond the normal idea of business software and build unique and creative solutions for your company. Check out this video for an example of just how far you can take it.

While it’s truly amazing that you can integrate your Salesforce data with Minecraft, there are also many practical applications for the API. Every time you use Salesforce, whether you’re using standard functionality or building a custom app, you’re interacting with the API.

## Resources
- [trust.salesforce.com](https://trust.salesforce.com/)
- [Lightning Platform Overview](https://developer.salesforce.com/platform/force.com)
- [Salesforce Developers Blog: Visualizing Data... in Minecraft!?](https://developer.salesforce.com/blogs/developer-relations/2014/01/visualizing-salesforce-data-in-minecraft.html)

## Copyright
Rights of ALBERT EINSTEIN are used with permission of The Hebrew University of Jerusalem. Represented exclusively by Greenlight.

## Quiz

**+100 points**

>**1**-Our trusted, multitenant cloud means you get:

**A.**The benefits of the same core set of features for all customers

**B.**Upgrades three times a year

**C.**No software to install to access Salesforce

==**D.**All of the above==

> **2**-The Salesforce API is:

==**A.**Like a contract between two pieces of software, allowing them to connect and exchange information==

**B.**Not available for certain technologies such as wearables

**C.**The exact same thing as an API name

**D.**Only for programmers to use

> **3**-Metadata refers to:

**A.**Everything in your Salesforce org, including your customer and user data

**B.**A representation of your standard functionality, without customizations

==**C.**Data about data==

**D.**Configuration-based modifications only

Check the Quiz to Earn 100 Points

Second attempt earns 50 points. Three or more earns 25 points.