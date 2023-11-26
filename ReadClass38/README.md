# Read Class - 38

**What are the three criteria an acticity’s intent filter must fulfill in order for a system to send an intent to that activity?**

Intent filters are a crucial mechanism in Android development for defining how an activity responds to incoming intents. They act as filters, sifting through intents and directing them to the appropriate components. To fulfill their purpose, an activity's intent filter must adhere to three essential criteria:

1. **Action:** The intent filter must specify the action that the activity can handle. This action serves as a general identifier for the type of task the intent is meant to perform.

2. **Data:** The intent filter can also define the data type that the activity is designed to process. This data provides additional context about the intent's purpose and allows for more refined filtering.

3. **Categories:** Categories provide further context and categorization for intents. They can be used to group related intents together or to indicate specific aspects of the intent's purpose.

**How does an activity retrieve the Intent that it was started by?**

When an activity is launched through an intent, the system automatically passes the intent object to the activity's `onCreate()` method. To retrieve this intent object, the activity can use the `getIntent()` method. This method provides access to the intent's contents, including the action, data, and categories.

**Explain intents to a non-technical friend.**

Imagine you're sending a message to a friend. The message itself is like an intent, carrying information from you (the sender) to your friend (the receiver). Intents in Android work similarly. They carry data and instructions from one part of the app to another, specifying what action to take and what data to process.

**Compare and contrast implicit and explicit intents.**

Implicit intents are like open invitations, sent out to any app that can handle them. They don't specify a particular app but rather broadcast the intent to all potential receivers. The system then selects the most appropriate app to handle the intent based on its intent filter.

Explicit intents, on the other hand, are like direct invitations, addressed to a specific app. They explicitly specify the name of the app they want to launch, leaving no room for ambiguity. This approach is useful when you know exactly which app you want to handle the intent.

**What is the primary information contained within an Intent?**

An intent primarily carries three pieces of information:

1. **Component nam**

2. **Action**

3. **Data**

4. **Category**

5. **Extras**

6. **Flags**
