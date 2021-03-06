# java-appium-automation

This repository demonstrates how to run Appium Java tests on Protean App Automate.

## Setup

### Requirements

**1. Java 8+**

- If Java is not installed, follow these instructions:
- For Windows, download latest java version from [here](https://java.com/en/download/) and run the installer executable
- For Mac and Linux, run `java -version` to see what java version is pre-installed. If you want a different version download from [here](https://java.com/en/download/)

**2. Maven**
   - If you want to run automation from Maven project, you need to install Maven
   - If Maven is not downloaded, download it from [here](https://maven.apache.org/download.cgi)
   - For installation, follow the instructions [here](https://maven.apache.org/install.html)

### Install the dependencies

To install the dependencies, run the following command in the project's base folder

```cmd
mvn clean install
```

## Getting Started

- Getting Started with Appium tests in Java on Protean is that simple! :

**1. For Maven Project**
- Put the following dependency in your pom.xml file along with selenium dependency [here](https://mvnrepository.com/artifact/io.appium/java-client/7.0.0)

**2. For Java Project**

- Download appium java-client from [here](https://mvnrepository.com/artifact/io.appium/java-client/7.0.0) and put in your dependency file (build path)

### Run your first test :

**1. Upload your Android or iOS App**

Upload and install your Android app (.apk or .aab file) or iOS app (.ipa file) to Protean servers from upload app section of Dashboard tab.


**2. Configure and run your first test**

Open `AppiumTest.java` file in the `android` directory :

- Replace `YOUR_USERNAME` & `YOUR_ACCESS_KEY` with your Protean access credentials. 
	
 `USERNAME` is Protean login id / email.
 
 You can get `ACCESS_KEY` from `keys` section of `Settings` tab of Protean App.

- Replace `Custom_AppPackage` & `Custom_AppActivity` with the correct app details.

- Replace `Device_Name`, `UDID`(Serial No of device), `Platform_Name`(Android/IOS), `Platform_Version` and `Test_Name`(Any name)

- Write test script for your app

- Run the test

- You can access the test execution results on [Automation --> Automation_Logs tab]

---

### Find Elements of mobile
- Go to `Automation` tab.
- Click on `Start app Inspector` button, then app inspector window will open on next tab.
- Go to mobile screen and go to page where you want to find locator of element.
- Now go to app inspector tab and `refresh it`.
- Mobile screen with your elemwnt will appear, now click on the element which you want to locate, then you will find all loactors of that element on right side of that mobile screen.
- Copy locator which you want and paste it on your script.
- You can also find `appPackage` in this tab.
