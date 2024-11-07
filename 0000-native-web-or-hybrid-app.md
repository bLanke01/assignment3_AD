# 0 - Native web or hybrid app

* Status: accepted 
* Deciders: everyone 
* Template used: [MADR 3.0.0](https://adr.github.io/madr/) 


## Context and Problem Statement

Determining which platform is best for the mobile music player app. Must provide a smooth user 	experience with no performance issues. 

## Considered Options

* Native App (iOS & Android) only. 
* Web App only. 
* Hybrid App.

## Decision Outcome

The decision was made to develop a hybrid music player app using Xamarin. 

## Rationale

* Xamarin supports native-like performance and cross-platform compatibility, reducing development time and costs. 
* Targeting both native and web platforms maximizes the potential user base. 
* Cross-platform functionality / compatibility. Users may have diverse preferences; switching the source of their music from a mobile application to a web application when they are on a laptop / desktop device (ex. Spotify, YouTube Music, etc.). 
* Can enable music download, or other offline features for a better user experience 

### Consequences 

* Cost-effective approach to cross platform compatibility. 
* Must provide consistent UI/UX across both web and native platforms. 
* Development and testing efforts increase for hybrid platform support 
* Slightly less-optimal performance compared to a full native application. 
* Complex code customization 

## Follow-Up Actions

* Identify and address platform-specific design (iOS, android, web) and development considerations. 
* Initial application prototype-building via Xamarin. 
* Regularly test and optimize the hybrid music player app’s performance and functionality. 
* Identify platform-specific functionalities for iOS, android, and web. 

