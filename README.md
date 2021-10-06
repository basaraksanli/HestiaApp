## Hestia
![Latest Version](https://img.shields.io/badge/latestVersion-1.0-yellow) ![Kotlin](https://img.shields.io/badge/language-kotlin-blue) ![Minimum SDK Version](https://img.shields.io/badge/minSDK-26-orange) ![Android Gradle Version](https://img.shields.io/badge/androidGradleVersion-4.1.1-green) ![Gradle Version](https://img.shields.io/badge/gradleVersion-6.5-informational)

<img src="/screenshots/1.png" width=350></img>
<img src="/screenshots/2.png" width=800></img>

## Introduction

Hestia is an Android application that provides users to share their locations with each other and chat either peer-to-peer or in groups. Hestia uses Huawei Mobile Services (HMS). In the application, users can add contacts by searching them by their e-mail address. Users can share their location and current activity with their selected contacts under limited duration and also can stop sharing their location and activity any time they need to. Each contact’s location is shown in Huawei Map alongside his or her current activity.

To accomplish to develop a chat and location sharing feature, Hestia uses Huawei Mobile Services. Among HMS Kits, we used Account Kit and Auth Service for sign-in operation. To keep user data, chat groups and messages, and also location-related information, Cloud DB is used. For location and activity related operations, Location Kit is implemented. To show push notification both for new message and location sharing information Push Kit and Cloud Functions are used together.

Alongside Hestia application, two libraries are developed; one for messaging and another for location sharing. These libraries are used to design and develop Hestia full reference app. 

## About HUAWEI Account Kit

The Account Kit provides easy, safe and fast registration to the user. Users can simply touch the Sign In with HUAWEI ID button to sign in with their HUAWEI IDs in the app easily and safely rather than inserting their credentials and wasting their time for authentication. To discover more, visit: [Huawei Account Kit Guide](https://developer.huawei.com/consumer/en/doc/development/HMSCore-Guides/introduction-0000001050048870)

## About HUAWEI Auth Service

Auth service provides multiple authentication methods to help developers secure user data based on simple rules. Developers can involve one or more of the authentication methods into their applications by using the AppGallery Auth Service SDK to accomplish quick and reliable registration and sign-in for users. To discover more, visit: [Huawei Auth Service Guide](https://developer.huawei.com/consumer/en/doc/development/AppGallery-connect-Guides/agc-auth-introduction-0000001053732605)

## About HUAWEI Cloud DB

Cloud DB is a device-cloud synergy database product that provides data synergy management capabilities between the device and cloud, unified data models, and various data management APIs. In addition to ensuring data availability, reliability, consistency, and security, CloudDB enables seamless data synchronization between the device and cloud, and supports offline application operations, helping developers quickly develop device-cloud and multi-device synergy applications. To discover more, visit: [Huawei Cloud DB Guide](https://developer.huawei.com/consumer/en/doc/development/AppGallery-connect-Guides/agc-clouddb-introduction)

## About HUAWEI Map Kit

Map Kit is an SDK for map development. It covers map data of more than 200 countries and regions, and supports over one hundred of languages. With this SDK, the developers can easily integrate map-based functions into their apps. To discover more, visit: [Huawei Map Kit Guide](https://developer.huawei.com/consumer/en/doc/development/HMSCore-Guides-V5/android-sdk-brief-introduction-0000001061991343-V5)

## About HUAWEI Location Kit

Location Kit combines the GNSS, Wi-Fi, and base station location functionalities into the apps to build up global positioning capabilities, allowing the developers to provide flexible location-based services for global users. Currently, it provides three main capabilities: fused location, activity identification, and geofence. You can call one or more of these capabilities as needed. To discover more, visit: [Huawei Location Kit Guide](https://developer.huawei.com/consumer/en/doc/development/HMSCore-Guides/introduction-0000001050706106)

## About Huawei Cloud Functions

Cloud Functions enables serverless computing. It provides the Function as a Service (FaaS) capabilities to simplify app development and O&M by splitting service logic into functions and offers the Cloud Functions SDK that works with Cloud DB and Cloud Storage so that your app functions can be implemented more easily. Cloud Functions automatically scales in or out functions based on actual traffic, freeing you from server resource management and helping you reduce costs. To discover more, visit: [Huawei Cloud Functions Guide](https://developer.huawei.com/consumer/en/doc/development/AppGallery-connect-Guides/agc-cloudfunction-introduction)

## What You Will Need

**Hardware Requirements**
- A computer that can run Android Studio.
- A Huawei Phone for debugging.

**Software Requirements**
- Android SDK package
- Android Studio 3.X-4.X
- HUAWEI HMS Core 4.0.2.300 or later
- JDK version: 1.8.211 or later
## Getting Started

Hestia uses HUAWEI services. In order to use them, you have to [create an app](https://developer.huawei.com/consumer/en/doc/distribution/app/agc-create_app) first. Before getting started, please [sign-up](https://id1.cloud.huawei.com/CAS/portal/userRegister/regbyemail.html?service=https%3A%2F%2Foauth-login1.cloud.huawei.com%2Foauth2%2Fv2%2Flogin%3Faccess_type%3Doffline%26client_id%3D6099200%26display%3Dpage%26flowID%3D6d751ab7-28c0-403c-a7a8-6fc07681a45d%26h%3D1603370512.3540%26lang%3Den-us%26redirect_uri%3Dhttps%253A%252F%252Fdeveloper.huawei.com%252Fconsumer%252Fen%252Flogin%252Fhtml%252FhandleLogin.html%26response_type%3Dcode%26scope%3Dopenid%2Bhttps%253A%252F%252Fwww.huawei.com%252Fauth%252Faccount%252Fcountry%2Bhttps%253A%252F%252Fwww.huawei.com%252Fauth%252Faccount%252Fbase.profile%26v%3D9f7b3af3ae56ae58c5cb23a5c1ff5af7d91720cea9a897be58cff23593e8c1ed&loginUrl=https%3A%2F%2Fid1.cloud.huawei.com%3A443%2FCAS%2Fportal%2FloginAuth.html&clientID=6099200&lang=en-us&display=page&loginChannel=89000060&reqClientType=89) for a HUAWEI developer account.

After creating the application, you need to [generate a signing certificate fingerprint](https://developer.huawei.com/consumer/en/codelab/HMSPreparation/index.html#3). Then you have to set this fingerprint to the application you created in AppGallery Connect.
- Go to "My Projects" in AppGallery Connect.
- Find your project from the project list and click the app on the project card.
- On the Project Setting page, set SHA-256 certificate fingerprint to the SHA-256 fingerprint you've generated.
![AGC-Fingerprint](https://communityfile-drcn.op.hicloud.com/FileServer/getFile/cmtyPub/011/111/111/0000000000011111111.20200511174103.08977471998788006824067329965155:50510612082412:2800:6930AD86F3F5AF6B2740EF666A56165E65A37E64FA305A30C5EFB998DA38D409.png?needInitFileName=true?needInitFileName=true?needInitFileName=true?needInitFileName=true)

## Using the Application

After starting the application, the first shown screen is the Splash screen. There, initialization of Cloud DB is done and also application check whether the user is already logged in or has to log in. If the user has to login, then the user is redirected to the Login screen. Currently, there is only Huawei login option available. In the future, more login options can be integrated due to the architectural structure of the login.

After the login screen, the Home screen is shown. If the user is already logged in, directly after the Splash screen Home screen opens, instead of Login. On the Home page, the user sees a map. After getting location related permissions, the user’s location is detected and that location is zoomed in on the map. Due to having a navigation drawer, the user reaches on settings and log out options via touching on the drawer which is half translucent on the top left of the page.

At the bottom of the page, there is a bottom sheet component. To contact user's connections s/he slides the bottom sheet up. The bottom sheet contains two tabs; one is for the list of contacts, and the other is for the list of groups. There the user can view her contacts on the left side of the tab which is under the title of People. The user can touch on the floating action button to add more contacts through the contacts page. To accomplish this, the user needs to know his/her contact’s email address. Via email address, the user can find her contact and add it to his/her contacts list which is shown on the People tab of the Home page.

On the right tab, which is called Groups, the user can create a group. The user can add anyone from his/her contacts into the group. The user can also add or change the photo of the group.

Both People and Groups tabs have similar interfaces, consisting of two options; one for location sharing and another for chatting. If the user presses the messaging icon, the chat page inside the bottom sheet appears. On the right top of the page, the participants of the chat are shown in the translucent list. That list shows only the profile pictures of the participants. The layout of the list comes in and goes out with animation depending on the entrance and exit of the chat page. If the user presses on the location icon, a dialog is opened showing location sharing duration options. Depending on the selected duration, his\her current location is shared either with his\her direct contact (peer-to-peer) or with his\her group. If the user contacts shared their location with his\her, then s\he can see his\her contact’s location on the map. Anytime the user can stop sharing location independent from the duration s\he selected before.

## Project Structure

Hestia App is designed with MVVM design pattern.

## Libraries

- Huawei Account Kit
- Huawei Auth Service
- Huawei Map Kit
- Huawei Location Kit
- Huawei Cloud DB
- Huawei Cloud Functions
- Material
- LiveData
- Kotlin Library
- Lifecycle
- Facebook Sign in
- CardView
- DataBinding
- Navigation
- Glide
- Preference
- Lottie
- Work Manager
- Vdurmont Emoji

## Contributors

- Cihan Yurtseven
- Ferid Cafer
- Basar Aksanli
- Oguzhan Demirci
- Sinan Yilmaz
- Sezer Bozkir
- Enes Kocaman

## License

Copyright 2021. Huawei Technologies Co., Ltd. All rights reserved.

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
