# ezXSS
ezXSS is an easy way for penetration testers and bug bounty hunters to test (blind) Cross Site Scripting.

## Docker Version
This fork is for a docker container. Need to use PHP 5.7 due to mysql8 default authentication changes. And setting docker-compose 'command' setting did not work :(

Run with docker-compose up --build

Note: This is not a secure production ready Docker deployment, so fix the mysql issues and secure the image.

## Current features
Some features ezXSS has

* Easy to use dashboard with statics, payloads, view/share/search reports and more
* Payload generator
* Instant email alert on payload
* Custom javascript payload
* Enable/Disable screenshots
* Prevent double payloads from saving or alerting
* Block domains 
* Share reports with a direct link or with other ezXSS users
* Easily manage and view reports in the dashboard
* Secure your login with extra protection (2FA)
* The following information is collected on a vulnerable page:
    * The URL of the page
    * IP Address
    * Any page referer (or share referer)
    * The User-Agent
    * All Non-HTTP-Only Cookies
    * All Locale Storage
    * All Session Storage
    * Full HTML DOM source of the page
    * Page origin
    * Time of execution
    * Screenshot of the page
* its just ez :-)

## Required
* A host with PHP 7.1 or up
* A domain name (consider a short one)
* An SSL if you want to test on https websites (consider Cloudflare or Let's Encrypt for a free SSL)

## Installation
ezXSS is ez to install

* Clone the repository and put the files in the document root
* Create an empty database and provide your database information in 'src/Database.php'
* Visit /manage/install in your browser and setup a password and email
* Done! That was ez right?

## Demo
For a demo visit [demo.ezxss.com/manage](https://demo.ezxss.com/manage) with password *demo1234*. Please note that some features might be disabled in the demo version.

## Screenshots

![Dashboard](https://i.imgur.com/79wSggJ.png)
![Settings](https://i.imgur.com/oybLHTn.png)
![Payload](https://i.imgur.com/Aibuvzz.png)
![Reports](https://i.imgur.com/xT1MmO1.png)
![Login](https://i.imgur.com/bEzskKo.png)
