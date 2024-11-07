# 3 - Permissions

* Status: accepted 
* Deciders: everyone 
* Template used: [MADR 3.0.0](https://adr.github.io/madr/) 


## Context and Problem Statement

* The music player app requires permissions for media storage(to play local files), internet access(for streaming musics) and optional user data (for personalization). This will ensure privacy, minimizing permissions, and complying with app store policies are essential goals. 

## Considered Options

* Request All Permissions When App Starts. 
* Request Permissions Only When Needed.  
* Provide a Settings Option When Initially Decline.   

## Decision Outcome

* Choosing Request Permissions Only When Needed is the best option so the users will be prompted for permission only when they try to use features that require them, such as accessing local music files or streaming music online. 

## Rationale

* Minimize user concerns about privacy by only requesting permissions when they are relevant which lead to building trust with the user. 
* Aligns with app store guidelines. 
* Reducing initial friction for users who may want to explore the app without granting full permissions immediately.  

### Consequences 

* Improved user trusts 
* Potential higher app store approval ratings  

## Follow-Up Actions

* Test every feature to ensure permissions are properly working. 
* Create a simple guide in the app’s settings to help users manage permissions. 
* Review app store guidelines to ensure compliance with privacy policies. 