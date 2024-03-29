﻿# MVC-Explained
This lecture serves to explain the MVC in a beginner friendly manner

# What is MVC ? 
MVC (Model-View-Controller) is a pattern in software design commonly used to implement user interfaces, data, and controlling logic. It emphasizes a separation between the software's business logic and display. This "separation of concerns" provides for a better division of labor and improved maintenance.

<div style="background: white; margin-bottom: 25px">
  <img src="https://www.freecodecamp.org/news/content/images/2021/04/MVC3.png" alt="MVC diagram">
</div>

# The Model
The model defines what data the app should contain. If the state of this data changes, then the model will usually notify the view (so the display can change as needed) and sometimes the controller (if different logic is needed to control the updated view).

### Database Schema 
se schema defines how data is organized within a relational database; this is inclusive of logical constraints such as, table names, fields, data types, and the relationships between these entities. Schemas commonly use visual representations to communicate the architecture of the database, becoming the foundation for an organization’s data management discipline. This process of database schema design is also known as data modeling.

These data models serve a variety of roles, such as database users, database administrators, and programmers. For example, it can help database administrators manage normalization processes to avoid data duplication. Alternatively, it can enable analysts to navigate these data structures to conduct reporting or other valuable business analyses. These diagrams act as valuable documentation within the database management system (DBMS), ensuring alignment across various stakeholders.

### Database schema vs. database instance

A database schema is considered the “blueprint” of a database which describes how the data may relate to other tables or other data models. However, the schema does not actually contain data.

A sample of data from a database at a single moment in time is known as a database instance. It contains all the properties that the schema describes as data values. Since database instances are just a snapshot at a given moment, they’re likely to change over time, unlike database schemas.

# The View
The view defines how the app's data should be displayed.

If we have a shopping list app, the view would define how the list is presented to the user, and receive the data to display from the model.

# The Controller
The controller contains logic that updates the model and/or view in response to input from the users of the app.

So for example, our shopping list could have input forms and buttons that allow us to add or delete items. These actions require the model to be updated, so the input is sent to the controller, which then manipulates the model as appropriate, which then sends updated data to the view.

You might however also want to just update the view to display the data in a different format, e.g., change the item order to alphabetical, or lowest to highest price. In this case the controller could handle this directly without needing to update the model.

# Example 
<div style="background: white; margin-bottom: 25px">
  <img src="https://www.guru99.com/images/1/122118_0445_MVCTutorial3.png" alt="">
</div>

## Car driving mechanism is an example of the MVC model.

#### Every car consist of three main parts :
- View = User interface : (Gear lever, panels, steering wheel, brake, etc.)
- Controller- Mechanism (Engine)
- Model- Storage (Petrol or Diesel tank)

#### The car runs from the engine and takes fuel from storage, but it can only be operated using the specified user interface devices

# Why Should You Use MVC?
Three words: separation of concerns, or SoC for short.

The MVC pattern helps you break up the frontend and backend code into separate components. This way, it's much easier to manage and make changes to either side without them interfering with each other.

But this is easier said than done, especially when several developers need to update, modify, or debug a full-blown application simultaneously.
