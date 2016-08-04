IBM MobileFirst Foundation 8.0
===
## Limit the number of devices per authenticated user
This sample shows how to limit the number of devices per authenticated user. The sample contains one security check - [UserLoginWithMaxDevicesSecurityCheck](/UserLoginWithMaxDevicesSecurityCheck).
This Security Check extends the simple [UserLogin Security Check](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/authentication-and-security/user-authentication/security-check/) adding logic to check how many devices the user is logged in on, and to either block the user from logging in on an additional device, beyond the max devices limit, or to automatically log them out of a different device when they try to log in from a new one.

The Security Check lets you configure the defaults for:
- Number of authenticated devices allowed per user - `Max Devices`.
- What action to take if the limit is reached: block current login or auto logout one of the authenticated devices. - `Auto Logout`.

##Demo
[![Limit the device number per authenticated user](https://img.youtube.com/vi/B_Hldzr8KAQ/0.jpg)](https://www.youtube.com/watch?v=B_Hldzr8KAQ)

### Prerequisites
1. Understanding the IBM MobileFirst Platform [Authentication and Security](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/authentication-and-security/).
2. Understanding the IBM MobileFirst Platform [Java Adapters](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/adapters/java-adapters/).
3. Pre-installed IBM MobileFirst Platform [development environment](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/setting-up-your-development-environment/).

### Usage

* Deploying the Security Check Adapter [UserLoginWithMaxDevicesSecurityCheck](/UserLoginWithMaxDevicesSecurityCheck) by use either Maven or MobileFirst Developer CLI to [build and deploy adapters](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/adapters/creating-adapters/).

* To test the sample Security Check Adapter use the [following tutorial](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/authentication-and-security/user-authentication/javascript/#sample-applications), but instead of using the UserLogin Security Check, use the current sample's Security Check ->  [UserLoginWithMaxDevicesSecurityCheck](/UserLoginWithMaxDevicesSecurityCheck).


### Supported Levels
IBM MobileFirst Platform Foundation 8.0

### License
Copyright 2016 IBM Corp.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
