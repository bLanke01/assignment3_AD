# 4 - Data Storage

* Status: accepted 
* Deciders: everyone 
* Template used: [MADR 3.0.0](https://adr.github.io/madr/) 


## Context and Problem Statement

The music player app will store various data types, including user information, playlists, music preferences, and possibly offline music files. The chosen storage solution should ensure scalability, fast data retrieval, and data integrity. Data security and privacy are also key, given that sensitive user data (e.g., login credentials) will be handled. The app requires a storage solution that integrates smoothly with the backend and supports cross-platform accessibility.

## Considered Options

* Cloud Storage  
* Local Device Storage  

## Decision Outcome

* Use cloud storage for storing user data, playlists, and media files, while leveraging local device storage for offline caching and playback.

## Rationale

* Cloud Storage is reliable for storing and syncing user data across devices, providing a central source of truth that is accessible anywhere with an internet connection. It’s also scalable, meaning that as the app’s user base grows, it can handle increasing amounts of data. 
* Local Device Storage is necessary for providing offline access and improving user experience by allowing users to cache music files and playlists for smoother, uninterrupted playback without needing to use mobile data. 

### Consequences 

* Scalability: Cloud storage solutions like AWS S3 or Google Cloud Storage offer high scalability but may incur costs based on usage. 
* Performance: Users on slow or unstable networks may experience slower performance when streaming directly from the cloud. 
* Offline Storage Limitations: Local storage on user devices is limited, so large music libraries could consume significant space. 

## Follow-Up Actions

* Set Up Cloud Services: Configure a reliable cloud storage provider (e.g., AWS S3 or Firebase) to manage and secure user data. 
* Implement Caching Policies: Develop strategies for caching playlists and frequently played songs to optimize local storage usage. 
* Develop User-Controlled Storage Management: Allow users to control cached data, providing options to manage offline files, clear caches, and manage space. 