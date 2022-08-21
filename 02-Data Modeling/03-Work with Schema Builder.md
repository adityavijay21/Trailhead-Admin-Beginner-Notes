# Work with Schema Builder


## Learning Objectives
- Describe the advantages of using Schema Builder for data modeling.
- Use Schema Builder to create a schema for a given object model.
- Use Schema Builder to add a custom object to your schema.
- Use Schema Builder to add a custom field to your schema.



## See Your Data Model in Action
By now, you and D’Angelo have created a handful of custom objects, fields, and relationships. Your app’s data model is starting to get a little more complicated.

Schema Builder is a tool that lets you visualize and edit your data model. It’s useful for designing and understanding complex data models like the one D’Angelo is building. Let’s take a look.

1. From Setup, search for and click Schema Builder in the Quick Find box. ![Quick Find box location.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/schema_builder/images/c717913268e0d4404b13777442f9e3b7_data-modeling-view-quick-find.png)
2. In the left panel, click **Clear All**.
3. Check Contact, Favorite, Offer, and Property. You should have the Favorite object from the previous unit, and the Offer and Property objects from the previous challenges.
4. Click **Auto-Layout**.

You'll see something like this:

![The user interface for the Schema Builder.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/schema_builder/images/eb1a1069fd6a29204a31dc7594295402_data-modeling-schema-ui.png)

Notice that you can drag these objects around the canvas. This doesn’t change your objects or relationships, but it can help you visualize your data model in a useful way. Schema Builder is a handy tool for introducing your Salesforce customizations to a co-worker or explaining the way data flows throughout your system.

![D'Angelo explaining the DreamHouse app schema to Michelle.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/schema_builder/images/dace12db4f5386c9f11691d47d1d1751_data-modeling-schema-expl.png)



## Create an Object with Schema Builder
You can also create objects using Schema Builder. If you prefer, you can create objects in this visual interface if you’re designing your system and want to be able to revise all your customizations on the spot. Let’s see how it’s done.

1. In the left sidebar, click the **Elements** tab.
2. Click **Object** and drag it onto the canvas.
3. Enter information about your object. You can make it whatever you want!
4. Click **Save**.

Your new object appears in the Schema Builder. That was quick! Next, let’s add some fields.



## Create Fields with Schema Builder
Creating fields with Schema Builder is just like creating objects.

1. From the Elements tab, choose a field type and drag it onto the object you just created. Notice that you can create relationship fields, formula fields, and normal fields in Schema Builder.
2. Fill out the details about your new field.
3. Click **Save**.

Cool! If you go back through Object Manager, you’ll see your new object shows up the same way your Property, Offer, and Favorite objects do.

![A comparison of an object in Object Manager and Schema Builder.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/schema_builder/images/1b6735e5fc2dbf913bbc29ac822a7b09_data-modeling-schema-create.png)



## Sum It Up
We’ve learned a lot in this module. First, we talked about the data model and the database. We covered objects, fields, and records and created some of each for our DreamHouse app. Then we talked about relationships between objects and how you can visualize your data model using Schema Builder.

As you start to dive into more advanced content, you’ll see custom objects and fields everywhere. Before you know it, you’ll be a data modeling pro. Happy building!


## Resources
- [*Salesforce Help*: Design Your Own Data Model](https://help.salesforce.com/articleView?id=schema_builder.htm&language=en_US)
- [*Salesforce Help*: Schema Builder Custom Object Reference](https://help.salesforce.com/articleView?id=schema_builder_elements_objects_ref.htm&language=en_US)

## Hands-on Challenge

**+500 points**

### GET READY

You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE

Use Schema Builder to create a custom field for the Property object

DreamHouse brokers often visit properties with their clients. They want to see on the property record where the property is located. Use Schema Builder to add a street address field to the Property object.

- Data Type: **Text Area**
- Field Label: **Street Address**
- Field Name: `Street_Address`
- Always require a value in this field in order to save a record: **Selected**