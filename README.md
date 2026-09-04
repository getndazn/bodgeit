![No longer maintained](https://img.shields.io/badge/Maintenance-OFF-red.svg)

### ⚠️ Deprecated

This repository is no longer actively maintained and has been archived by the [Security team](https://teams.microsoft.com/l/channel/19%3A38b4a7fa05ac4ec782143b767304c53c%40thread.skype/General?groupId=99480e15-059f-4bea-b7cc-4912903bd6f6&tenantId=30459df5-1e53-4d8b-a162-0ad2348546f1).
The repository is retained for historical and reference purposes and is read-only while archived.
If this repository is required in the future, it can be unarchived. Please raise a request with the [CodX team](https://teams.microsoft.com/l/channel/19%3Aa654db0c76f84164aebe0cccf297e6de%40thread.skype/CoDX%20Support?groupId=602f2603-465a-49fa-be9e-abfe0b05b551&tenantId=30459df5-1e53-4d8b-a162-0ad2348546f1) to have it unarchived.

The BodgeIt Store is a vulnerable web application which is currently aimed at people who are new to pen testing.

> ### Please note that The BodgeIt Store is no longer being worked on
> #### You are strongly recommended to use [OWASP Juice Shop](https://www.owasp.org/index.php/OWASP_Juice_Shop_Project) instead!

Note that the BodgeIt Store is now available as a Docker image: https://hub.docker.com/r/psiinon/bodgeit/ 

Some of its features and characteristics:
* Easy to install - just requires java and a servlet engine, e.g. Tomcat
* Self contained (no additional dependencies other than to 2 in the above line)
* Easy to change on the fly - all the functionality is implemented in JSPs, so no IDE required
* Cross platform
* Open source
* No separate db to install and configure - it uses an 'in memory' db that is automatically (re)initialized on start up

All you need to do is download and open the zip file, and then extract the war file into the webapps directory of your favorite servlet engine.

Then point your browser at (for example) http://localhost:8080/bodgeit

You may find it easier to find vulnerabilities using a pen test tool.

If you dont have a favourite one, I'd recommend the [Zed Attack Proxy](https://www.owasp.org/index.php/ZAP) (for which I'm the project lead).

The Bodge It Store include the following significant vulnerabilities:
* Cross Site Scripting
* SQL injection
* Hidden (but unprotected) content
* Cross Site Request Forgery
* Debug code
* Insecure Object References
* Application logic vulnerabilities If you spot any others then let me know ;)

There is also a 'scoring' page (linked from the 'About Us' page) where you can see various hacking challenges and whether you have completed them or not.

In the relatively near future I'm hoping to add things like:
* Ajax requests
* More vulnerabilities (of course)

You can now also perform automated security regression tests on the Bodge It Store - see the wiki.

Any feedback (or offers of help to develop it further;) would be appreciated.
