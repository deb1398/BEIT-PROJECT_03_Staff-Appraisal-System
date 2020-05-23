**Staff Appraisal System** is an open source application. With a growing list of installable modules, the **appraisal system** allows faculty to self assess themselfs and give their report to the higher authority in this case it will be the HoD. **Staff appraisal system** is built by:
- Debashish Choudhury (http://github.com/deb1398)
- Utkarsh Naik (https://github.com/utkarsh17naik)
- Anagha Devade (https://github.com/adevade16)

Under the guidance of:
- Anagha Aher
- Vishal Badgujar (https://github.com/vishal003)

Staff Appraisal System focuses on a modular plugin system and uses NodeJs for server side script, Hbs tamplate engine along with MongoDB to store data.

## Installation

#### Manual Installation

1. Download and install the latest *Node.js* version.
2. Clone the repository and check out the master branch: `git clone https://github.com/adevade16/BEIT-PROJECT_04_Staff-Appraisal-System`
3. Enter the repository: `cd BEIT-PROJECT_04_Staff-Appraisal-System/`
4. Install and run the app with: `npm install && npm start` \
   For **Server Only** use: `npm install && node serveronly` .

**Important:** Make sure to add .env file in the root of the application. Make sure that you whitelist the interface/ip (`ipWhitelist`) in the server config where you have created the mongodb collection, otherwise it will not be allowed to connect to the server. You also need to set the local host `address` field to `0.0.0.0` in order to make it open for all the ports.

**Important:** Changes that need to be done in .env file is as shown below:

```
HOST = 5000 // or enter your own port
PASSWD = // Enter the password of your organizations gmail account.
DBPASS = // Enter your mongodb user password
```
PASSWD is required for password reset. A mail will be sent to user for password reset link. This mail will be sent by the Organization's email id, hence password is required.


## Configuration

### General

If you want to update your Appraisal System to the latest version, use your terminal to go to your BEIT-PROJECT_04_Staff-Appraisal-System folder and type the following command:

```bash
git pull && npm install
```

If you changed nothing more than the config or the modules, this should work without any problems.
Type `git status` to see your changes, if there are any, you can reset them with `git reset --hard`. After that, git pull should be possible.

## Contributing Guidelines

Contributions of all kinds are welcome, not only in the form of code but also with regards bug reports and documentation.

Please keep the following in mind:

- **Bug Reports**:  Make sure you're running the latest version. If the issue(s) still persist: please open a clearly documented issue with a clear title.
- **Minor Bug Fixes**: Please send a pull request with a clear explanation of the issue or a link to the issue it solves.
- **Major Bug Fixes**: please discuss your approach in an GitHub issue before you start to alter a big part of the code.
- **New Features**: please please discuss in a GitHub issue before you start to alter a big part of the code. Without discussion upfront, the pull request will not be accepted / merged.

Thanks for your help in making Staff Appraisal System better!

## Important
To run this application as soon as the system or pi3 boots up.. install pm3.
It as a node package for running the file automatically after booting up of OS(Rasbian). Through pm2 we can also specify time for every reboot.

> ~ Debashish Choudhury
> ~ Utkarsh Naik
> ~ Anagha Devade
> ~ Anagha Aher
> ~ Vishal Badgujar
