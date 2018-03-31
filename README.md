# Youtube-chatbot

## Youtube Recommend Chatbot in React Native

An AI-driving react native app with conversational UI. Powered by DialogFlow and Youtube API, available on Android and iOS, will extend to website and other conversational channel soon!

### Concept
People like to watch video in field in both which they already familiar with and they are not familiar with but interested in. Also, sometimes they want to take a look at the field they never experience.


This application want to make people easily browse videos in **3 different stages** and **make friends** based on their video preference!
1. Watch video they are familiar with (their preference)
2. Watch video they are not familiar with but have interest to take a look
3. Watch random video and explore new area!
4. Make friends based on their video taste

### Target Channels
* iOS
* Android
* Smart Speakers ()
* Smart AR glasses (Require Google Play Store license)
* Website
* Conversational channels (Facebook, Telegram, Slack)

### Implementation

#### Step 0 Design system
1. Draw the system structure draft
2. Design UI and userflow
3. Scope initial phases and future possiblility
4. Select useful react-native package and components

#### Step 1 Create Google Project
- Create Google Project in GCP developer console, enable APIs
    * DialogFlow API
    * Youtube API
    * Youtube OAuth 2.0
    * Firebase APIs as storage (TBD: Firebase Cloud Messanger in future)
- Download and import credential

#### Step 2 Create DialogFlow Agent
- Define intent and entities, function = Intent(arrt: entity)
    1. Preference_videos() // default, show videos in user's preference_list
    2. Search_video (video_name)
    3. Explore_videos() // Show videos in their explore_list
    4. Random_video() // show videos not in user's list
    5. Suggest_friend()
    6. Show_preference()
    7. Add_preference(preference_type)
    8. Delete_preference(preference_type)
    9. Show_explore()
    10. Add_explore(explore_type)
    11. Delete_explore(explore_type)
    
#### Step 3 Create UI Layout

* Create Splash screen
* Create Login page
* Create tabs and Chat page, Preference page, Explore page

#### Step 3 Connect user data with firebase

#### Step 4 Connect Youtube OAuth in Login page

#### Step 5 Connect Dialogflow Agent in Chat page

#### Step 6 Connect Youtube API and retrieve videos

    

### Select Packages
- React-native-Youtube
- React-native-OAuth
- React-native-DialogFlow
- Layout


### Reference
- Video sources: Youtube, The Movie Database(TMDb)
- Notification: Google Cloud Messaging, Firebase Cloud Messaging API


### Issues Log
1. DialogFlow is integration with Google Cloud, internal errors coming and cannot create project - "You've reached the limit of GCP projects" and cannot delete existing project - "Unknown error errorid=31b10631-5bac-4166-8f70-a0e01be900ad"
>> create a new google account 

### Current Status

