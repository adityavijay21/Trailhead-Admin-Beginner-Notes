# Create Object Relationships



## Learning Objectives
After completing this unit, you’ll be able to:

- Define the different types of object relationships and their typical use cases.
- Create or modify a lookup relationship.
- Create or modify a master-detail relationship.



## What Are Object Relationships?
Now that we’re comfortable with objects and fields, it’s time to take things to the next level with object relationships. Object relationships are a special field type that connects two objects together.

Let’s think about a standard object like Account. If a sales rep opens an account, they’ve probably been talking to a few people at that account’s company. They’ve probably made contacts like executives or IT managers and stored those contacts’ information in Salesforce.

It makes sense, then, that there should be a relationship between the Account object and the Contact object. And there is!

When you look at an account record in Salesforce, you can see that there’s a section for contacts on the Related tab. You can also see that there’s a button that lets you quickly add a contact to an account.

![An account record with two related contacts.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/object_relationships/images/e2f097878f8f051bfa2604edf31c0824_data-modeling-relationships-contacts.png)

The Account to Contact relationship is an example of a standard relationship in Salesforce. But just like objects and fields, you can build custom relationships as well. In the last unit, you created two objects: Property and Offer. Wouldn’t it be great if all the offers made on a home showed up on its record in Salesforce?

Before we do that, let’s talk about the different kinds of relationships you can create in Salesforce.



## The Wide World of Object Relationships
There are two main types of object relationships: lookup and master-detail.

**Lookup Relationships**

In our Account to Contact example above, ==the relationship between the two objects is a **lookup relationship**. A lookup relationship essentially links two objects together so that you can “look up” one object from the related items on another object.==

==Lookup relationships can be one-to-one or one-to-many. The Account to Contact relationship is one-to-many because a single account can have many related contacts. ==For our DreamHouse scenario, you could create a one-to-one relationship between the Property object and a Home Seller object.

**Master-Detail Relationships**

While lookup relationships are fairly casual, ==**master-detail relationships** are a bit tighter==. ==In this type of relationship, one object is the master and another is the detail. The master object controls certain behaviors of the detail object, like who can view the detail’s data.==

For example, let’s say the owner of a property wanted to take their home off the market. DreamHouse wouldn’t want to keep any offers made on that property. With a master-detail relationship between Property and Offer, you can delete the property and all its associated offers from your system.

![A property with several related offers.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/object_relationships/images/c2522a70dfde1c538e39b802d8cde60e_data-modeling-master-detail.png)


**More on Relationships**

Just like in real life, relationships are complicated. Here’s a bit more information to help you differentiate between lookup and master-detail relationships.

Typically, you use lookup relationships when objects are only related in some cases. Sometimes a contact is associated with a specific account, but sometimes it’s just a contact. Objects in lookup relationships usually work as stand-alone objects and have their own tabs in the user interface.

In a master-detail relationship, the detail object doesn’t work as a stand-alone. It’s highly dependent on the master. In fact, if a record on the master object is deleted, all its related detail records are deleted as well. When you’re creating master-detail relationships, you always create the relationship field on the detail object.

Finally, you could run into a third relationship type called a hierarchical relationship. Hierarchical relationships are a special type of lookup relationship. The main difference between the two is that hierarchical relationships are only available on the User object. You can use them for things like creating management chains between users.

When you start adding relationships between objects, remember that you’re increasing the complexity of your data model. That’s not a bad thing, but be extra cautious when you do things like change and delete objects, records, or fields. Check out the resources section for more information on relationship behaviors.



## Create a Custom Object
We’re ready to jump back in with D’Angelo to build some relationships for the DreamHouse app. Let’s say DreamHouse wanted a way to track users who favorite properties on their website. This feature can help DreamHouse’s real estate brokers reach out to potential home buyers.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Even if you're completing this module as part of the Admin Beginner trail, be sure you use the new Trailhead Playground you created in the previous unit.

To start, create a custom object called Favorite and add a field to the object.

1. Click the **Object Manager** tab.
2. Click **Create** | **Custom Object** in the top-right corner.
3. For Label, enter `Favorite`.
4. For Plural Label, enter `Favorites`.
5. Check the box for **Launch New Custom Tab Wizard after saving this custom object**.
6. Leave the rest of the values as default and click **Save**.
7. On the New Custom Object Tab page, click the Tab Style field and select a style you like.
8. Click **Next**, **Next**, and **Save**.



## Create a Lookup Relationship
We’re going to create two custom relationship fields on the Favorite object. First, let’s create a lookup relationship that lists the users who select **Favorite** for a property.

1. From Setup, go to **Object Manager** | **Favorite**.
2. On the sidebar, click **Fields & Relationships**.
3. Click **New**.
4. Choose **Lookup Relationship** and click **Next**.
5. For Related To, choose **Contact**. For the purposes of DreamHouse, contacts represent potential home buyers.
6. Click **Next**.
7. For Field Name, enter Contact, then click **Next**.
8. Click **Next**, **Next**, and **Save**.



## Create a Master-Detail Relationship
Now, we’re going to create a second relationship field. We want a master-detail relationship where Property is the master and Favorite is the detail.

1. On the Object Manager page for the custom object, click **Fields & Relationships**.
2. Click **New**.
3. Select **Master-Detail Relationship** and click **Next**.
4. For Related To, choose **Property**.
5. Click **Next**.
6. For Field Name, enter `Property` and click **Next**.
7. Click **Next**, **Next**, and **Save**.

Now, if you look at a Property record, you’ll see Favorites listed in the related tab.

## Add a Favorite Property
Let's take a look at how to view favorite properties.

1. From the App Launcher (![The App Launcher icon.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/object_relationships/images/9d6dcd253b18771c09d19e84c34018bd_platform-basics-applauncher-2-2.png) in the navigation bar), find and select **Sales**.
2. Click the **Properties** tab in the navigation bar. If you don’t see it, look under the **More** dropdown.
3. Click the name of a Property record.
4. Click **Related**. You’ll see Favorites (0) in the related tab.
5. Click **New**.
6. Enter a name for Favorite Name, then click **Save**.

Great job! Our Favorite object is all set up.



## Resources
- [*Salesforce Help*: Object Relationships Overview](https://help.salesforce.com/articleView?id=overview_of_custom_object_relationships.htm&language=en_US)
- [*Salesforce Help*: Considerations for Relationship](https://help.salesforce.com/articleView?id=relationships_considerations.htm&language=en_US)

Where possible, we changed noninclusive terms to align with our company value of [Equality](https://help.salesforce.com/s/articleView?id=release-notes.rn_general_terms_replacement.htm&type=5&release=230). This is a work in progress, so if you find a term to evaluate for inclusive language, click **Provide feedback for this badge** in the right sidebar to submit it.

## Hands-on Challenge

**+500 points**

### GET READY

You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE

Create relationships for the Offer object

The object you created for the previous challenge is pretty handy. Imagine how much more useful it would be if brokers could specify which client made an offer and which property the client wants to buy. Add two relationships to the Offer object so brokers can capture this data in Salesforce. Create a Master-Detail relationship with the Property object and a Lookup relationship with the Contact object.

Even if you're completing this module as part of the Admin Beginner trail, be sure you use the new Trailhead Playground you created in the previous unit.
**Before You Start:**

- Create the **Property** object as described in the previous unit.


**Challenge Requirements:**

- Create a custom Master-Detail field on the Offer object
  - Data Type: **Master-Detail**
  - Field Label: **Property**
  - Field Name: `Property`
- Create a custom Lookup field on the Offer object
  - Data Type: **Lookup**
  - Field Label: **Contact**
  - Field Name: `Contact`