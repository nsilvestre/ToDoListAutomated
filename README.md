<!----- Conversion time: 9.122 seconds.


Using this Markdown file:

1. Cut and paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β17
* Thu May 30 2019 08:00:16 GMT-0700 (PDT)
* Source doc: https://docs.google.com/open?id=1n49Jyac1nYeKlnzaG-r7kyaNWU95Ig8fa5kDIE3SWOE
* This document has images: check for >>>>>  gd2md-html alert:  inline image link in generated source and store images to your server.
----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 0; ALERTS: 15.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>
<a href="#gdcalert4">alert4</a>
<a href="#gdcalert5">alert5</a>
<a href="#gdcalert6">alert6</a>
<a href="#gdcalert7">alert7</a>
<a href="#gdcalert8">alert8</a>
<a href="#gdcalert9">alert9</a>
<a href="#gdcalert10">alert10</a>
<a href="#gdcalert11">alert11</a>
<a href="#gdcalert12">alert12</a>
<a href="#gdcalert13">alert13</a>
<a href="#gdcalert14">alert14</a>
<a href="#gdcalert15">alert15</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



# **TAS (Test Automation Solution)**

This framework has been developed for internal use on Belatrix projects and adapted to EATSA necesites.

It uses **Java** as main language, **Cucumber **(_[https://cucumber.io/](https://cucumber.io/)_)** **and **Appium** (_http://appium.io_) for scenarios creation and Mobile testing and **RestAssured** (_http://rest-assured.io_) for API testing/actions. 


## 
Getting Started

These instructions will help you to get the project up and running on your local machine for development and testing purposes.


### 
**Prerequisites**


```
-Java JDK -> Java 11
-Brew
-Node -> v11.9.0
-Appium -> 1.10.1
-Carthage
-Maven
-IntelliJ IDEA
- Cucumber for Java plugin
- Gherkin plugin
-iOS Simulator
-App built to be used in a simulator
```



### 
**Installing**



*   **Java JDK**

Download it from:  \
<code>[https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html)</code>



*   **Install brew package manager.**

Open a terminal and execute the command:


```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

```



*   **Install Node.**

In the terminal execute: 


```
brew install node

```



*   **Install Appium.**

In a terminal run the following command:` `


```
npm install -g appium

```



*   **Install Carthage.**

In the same terminal execute the command:` `


```
brew install carthage

```



*   **Install Maven.**

Download the binary file from: 


```
https://maven.apache.org/download.cgi

```



*   **Install Intelllij IDEA.**

Download the Community version from: 


<code>[https://www.jetbrains.com/idea/download](https://www.jetbrains.com/idea/download)<strong> \
\
Set $JAVA_HOME environment variable</strong></code>


```
$ vim .bash_profile 
export JAVA_HOME=$(/usr/libexec/java_home)
$ source .bash_profile
$ echo $JAVA_HOME
```



<code>/Library/Java/JavaVirtualMachines/jdk-11.0.1.jdk/Contents/Home \
\
<strong>Import Project</strong></code>



1. TAS project is located on Kiosk project in a folder called **Automation-UITests **(_Kiosk/Automation-UITests_)
2. Open IntelliJ IDEA
3. Click Import Project option
4. Select the Automation-UITests folder
5. Select Maven \


<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme0.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme0.png "image_tooltip")

6. Click Next on following wizard page
7. Click Next on following wizard page
8. Select groupId \


<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme1.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme1.png "image_tooltip")

9. Select SDK \


<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme2.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme2.png "image_tooltip")

10. Confirm the project name

<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme3.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme3.png "image_tooltip")


## 
**Running the tests**


Tests can be run with Maven or JUnit.

\
[_Ideally following step won’t be needed in the near future_]

Regardless which method is chosen, the **app** capability that takes place in the .json configuration file inside the TAS needs to be be updated. This **app** capability must have the local path of the app under testing.

**_ \
_**Json file is located at:**_ \
`/Users/nsilvestre/Documents/EATSA/Kiosk/Kiosk/Automation-UITests/json_configs/appium_configs/eatsa_simulated_ipad_air_2.json`_**

\
Update app path: \
from:** \
`"app":"/Users/travis/build/Keenwawa/Kiosk/Kiosk_all_Debug_2.12.0_1329_test_simulator.app.zip"`** \
to:


```
"app":"/Users/nsilvestre/Documents/Apps/Kiosk_all_Debug_2.12.0_1329_test_simulator.app.zip"
```


**MAVEN:**



1. Open a terminal and launch the Appium server \
`$ appium`
2. To run the entire suite navigate to the TAS path and execute: \
`$ mvn test \
`

<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme4.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme4.png "image_tooltip")
` \
\
`

<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme5.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme5.png "image_tooltip")
` \
`

This command will execute the tests based on the configuration specified on TestRunner.java (_Kiosk/Automation-UITests/src/test/java/com/company/test/runner/TestRunner.java_) which by default is the entire suite (_features = {"src/test/java/com/company/test/features/EATSA"}_).


```


<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme6.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme6.png "image_tooltip")



```


If you want to execute just one or few feature files instead, you can do so:     \



`$ mvn test -Dcucumber.options="--glue com/company/test/steps/common/ --glue com/company/test/steps/EATSA src/test/java/com/company/test/features/EATSA/A_SetUp.feature src/test/java/com/company/test/features/EATSA/OutOfStocks.feature" \
\
`In this case just **A_SetUp.feature** (_it’s always needed for environment configuration purposes_) and **OutOfStocks.feature** will be executed.



3. Test results report can be found at: <code><em>Kiosk/Automation-UITests/</em>target/Eatsa/cucumber-report-html/cucumber-html-reports/</code>

<strong>JUnit: \
</strong>



1. From IntelliJ tap the following option on the right top corner: \


<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme7.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme7.png "image_tooltip")

2. Tap + button and JUnit: \


<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme8.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme8.png "image_tooltip")

3. Configuration:
1. Name: it represent the name of the feature/s you will be running. I.e: OutOfStocks, All, etc.
2. Test kind: _All in package_
3. Package: _com.company.test.runner_
4. VM options: it’s the same argument passed to Maven in the previous example: \
`-Dcucumber.options="--glue com/company/test/steps/common/ --glue com/company/test/steps/EATSA src/test/java/com/company/test/features/EATSA/A_SetUp.feature src/test/java/com/company/test/features/EATSA/OutOfStocks.feature"`

<code>         \
<em>Glue code: it's the code that interacts with the application. It's the implementation of the actions described on .feature files. \
</em></code>

5. Working directory: $MODULE_WORKING_DIR$
6. Use classpath of module: AutomationFramework
4. Run the test: \


<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme9.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme9.png "image_tooltip")


## 
**Project Structure**


Under Automation-UITests/src there are two main folders:



*   java
*   test

**Java**

This folder contains classes related with the Framework, system’s constants, main page object and utils. 

Subfolders:



*   base: framework-related classes. They are used to create the Appium Driver.
*   constants: system and domain constants.
*   pageobject: contains the main page object, _MobileBasePO_. All page object classes extends from this one. This class is responsible of Explicit Wait Driver creation.
*   utils: framework and domain util classes.
*   APIUtils: this class contains the methods to mark elements (items and modifiers) as Out of Stock.

**Test**

This folder contains all the stuff related with test cases creation.

Subfolders:



*   features: contains all the .features files
*   steps: contains the _glue_ code
*   pages: contains all the page objects

Above concepts (_features, steps, pages_) are explained in details in the following sections.


## 
**Cucumber**

**Introduction**

Cucumber is a tool that supports [Behaviour-Driven Development(BDD)](https://cucumber.io/docs/bdd).

Cucumber reads executable specifications written in plain text and validates that the software does what those specifications say. For example:


```
Scenario: Validate that email can be added/edited
When I swipe to login
And I navigate to the User Information screen
And I tap the email
And I enter an email
And I save the changes
Then the email is saved
```


Each scenario is a list of steps for Cucumber to work through. Cucumber verifies that the software conforms with the specification and generates a report indicating ✅ success or ❌ failure for each scenario.

In order for Cucumber to understand the scenarios, they must follow some basic syntax rules, called [Gherkin](https://cucumber.io/docs/gherkin/).

**What is Gherkin?**

Gherkin is a simple set of grammar rules that makes plain text structured enough for Cucumber to understand. The scenario above (_Validate that email can be added/edited_) is written in Gherkin.

Gherkin serves multiple purposes:



*   Unambiguous executable specification
*   Automated testing using Cucumber
*   Document how the system actually behaves



<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme10.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme10.png "image_tooltip")


Gherkin documents are stored in **.feature (src/test/features/)** text files.

It is strongly recommended to read the Gherkin keywords in order to understand, create and edit .features files:

[https://cucumber.io/docs/gherkin/reference/](https://cucumber.io/docs/gherkin/reference/). 

The most used in this project are:



*   Feature
*   Given, When, Then, And
*   Scenario Outline
*   Examples
*   Data Tables

**Step Definitions**

In addition to **[feature files](https://cucumber.io/docs/gherkin/reference#feature)** **(src/test/features/)**, Cucumber needs a set of **s[tep definitions](https://cucumber.io/docs/cucumber/step-definitions)** **(src/test/steps/)**. Step definitions map (or “**glue**”) each Gherkin step to programming code to carry out the action that should be performed by the step.

Step definitions hard-wire the specification to the implementation. For example:

The following Gherkin step in `Accountmanagement.feature` file:


```
When I swipe to login
```


Corresponds with the following step definition on `LoginSteps.java` file: \
**<code> \
@When("^I swipe to login$")</code></strong>


```
public void swipeToLogin() {
loginPage.swipeToLogin();
```


<code>}<strong><em> \
</em></strong></code>


## 
**Features, steps and page objects relation**

Each ‘**.feature file’** **(src/test/features/) **groups scenarios that are related and test one particular feature. For instance, `AddItemToCart.feature` has the following scenarios:



*   Add item from item details screen
*   Add item from force customize
*   Add item from re-order
*   Add item from details screen but accessing through re-order

On the other hand, each ‘**steps definitition file’** **(src/test/steps/) **groups the steps based on the following criterias:



*   The screen where the step applies to (most of the steps java file belong to this type): `ItemDetailsSteps.java, ItemListSteps.java, ForceCustomizeSteps.java, etc`
*   One particular feature from an external system:` OutOfSotcksSteps.java`
*   One particular View type, the alerts:` AlertsSteps.java`
*   Steps that apply in more than one screen:` EatsaUtilsSteps`

Per each ‘**steps definition class’** exists a ‘**page object class’ (src/test/pages/) **that implement each steps. For instance:

`ItemDetailsSteps.java` has two steps: \



```
@And("^I tap customize from Item Details screen")
public void iTapCustomizeFromItemDetailsScreen(){
itemDetailsPage.tapCustomize();
}

@And("^I tap add from Item Details screen")
public void iTapAddFromItemDetailsScreen(){
itemDetailsPage.tapAdd();
}
```


And the` ItemDetailsPage.java` has the implementation of those two steps:


```
public void tapCustomize() {
getWaitDriver().until(ExpectedConditions.elementToBeClickable(MobileBy.iOSNsPredicateString(customizePredicate))).click();
}

public void tapAdd() {
getWaitDriver().until(ExpectedConditions.elementToBeClickable(MobileBy.iOSNsPredicateString(addPredicate))).click();
}
```


So to sum up, **feature** files contains scenarios that are related to one feature. Each scenario has **steps** that are executed in different screens. Therefore, the** steps **of a scenario, are implemented in different **step definition** classes. Each **step definition** class corresponds to one **page **class (I.E: `CheckOutSteps.java -> CheckOutPage.java`).


## 
**Feature and Scenario creation**

**Path:** Automation-UITests/src/test/java/com.company.test/features

**Feature**

Each feature needs to start with the **Feature **keyword, follow by its name. The feature, is going to be identify in the reports by this name. Finally, after this line and before the first scenario, there’s a place for the description of the user story.

**Scenario**

Each scenario must start with the **Scenario Outline **keyword followed by a brief scenario description. **Scenario Outline **keyword works together with the **Examples **keywords, which is a table appended at the end of the scenario. 

The **Scenario Outline** keyword can be used to run the same Scenario multiple times, with different combinations of values. Those values are included as variables in the steps (_<config> and <partner> for below example_) and their values are specified in the Examples data table. The **Scenario Outline **will run one time per each row in the table passing the data of the row to the steps. In this way we can execute the same scenario multiple times just adding a new rows to the Examples table.


```
Feature: Account Management

As a user
I would like to have a Profile Screen
So that I can add/edit my Name and Email
and see my credit card numbers

Scenario Outline: Validate that name can be added/edited - DT
Given <config> appium driver

When I select <partner> partner
And I swipe to login
And I navigate to the User Information screen
And I tap the name
And I enter a name and last name
And I save the changes
Then the name is saved

Examples:
| config                     | partner |
| eatsa_simulated_iPad_air_2 | ROTI    |
| eatsa_simulated_iPad_air_2 | WOWBAO  |
```


**Important:**

Each scenario **must** start with the following **Given** step:


```
Given <config> appium driver
```


This step is used to create the **Appium driver** that is used along the scenario. This Appium driver is created based on the capabilities indicated in the **.json** file that is passed to the **Given** step through the **<config>** parameter:


```
Examples:
| config                     | 
| eatsa_simulated_iPad_air_2 | 
```


This .json indicate, among other things, the simulator (device name, platform version) in which the test will be executed. If you want to run the same scenario in a different device, add another .json file to Automation-UITests/json_configs/appium_configs, then add a new row to the examples table indicating the new .json and that’s it. You have one scenario running in two different platforms.

To summarize, each scenario **must** at least follow this main template:


```
Scenario Outline: _Scenario description_
Given <config> appium driver
```


.

.

Steps \
.

.


```
Examples:
| config                     | 
| eatsa_simulated_iPad_air_2 | 
```



## 
**Step Definition Class creation**

**Path:** Automation-UITests/src/test/java/com.company.test/steps

Each **step** class, in its constructor, needs to get the **driver** from the **context**, and create the **page **object that corresponds to this **Steps** class (_CheckOutSteps corresponds to CheckOutPage_):


```
public CheckOutSteps(Context context){
this.context = context;
driver = (AppiumDriver) context.getValue("driver");
checkOutPage = new CheckOutPage(driver);
}
```


Then, the **page** object is used among each step to invoke the actions that corresponds to the step and screen under testing:


```
@And("I pay the order$")
public void iPayOrder(){
checkOutPage.payOrder();
}
```


Full example of Steps definition class:


```
public class CheckOutSteps {

private final Context context;
private AppiumDriver driver;
private CheckOutPage checkOutPage;

public CheckOutSteps(Context context){
this.context = context;
driver = (AppiumDriver) context.getValue("driver");
checkOutPage = new CheckOutPage(driver);
}

@And("I pay the order$")
public void iPayOrder(){
checkOutPage.payOrder();
}

@And("^I tap the email from Checkout screen$")
public void iTapTheEmailFromCheckoutScreen() {
checkOutPage.tapEmail();
}

@Then("^the email is shown$")
public void theEmailIsShown() {
Assert.assertTrue(checkOutPage.validateEmailIsSaved());
}

}
```



## 
**Step definition method creation**

Each step on a .feature files must corresponds with a Step Definition (_the glue code_) in a steps class.

There are two very useful IntelliJ plugins that help us with this:



*   Cucumber for Java
*   Gherkin

Having those two plugins installed make a very nice test creation experience.

When a new line is added to a .feature file, the IDE automatically understands that it doesn’t have a step definition yet and marks it as such:



<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme11.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme11.png "image_tooltip")


Tapping Option+Enter we can display the possible actions:



<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme12.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme12.png "image_tooltip")


Selecting **create step definition** will prompt us to which step class we want to add the step and it will be automatically added following the Gherkin convention:



<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme13.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme13.png "image_tooltip")


If PartnerSteps is selected then the method is added there:



<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/TASReadme14.png). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/TASReadme14.png "image_tooltip")


Then inside the **iDoAnActionThatIsNotCreatedYet()** invoke the method in the page object and that’s it.

If the step has a variable like:


```
When I select <partner> partner
```


A cucumber expression needs to be indicated in the Step definition, and it’s automatically passed as a parameter to the method:


```
@When("^I select ([^\"]*) partner$")
public void iSelectPartnerPartner(String partner) {
partnersPage.selectPartner(partner);
}
```


There are several ways to do this depending on the parameter type. All the information is in below link: 



*   [https://cucumber.io/docs/cucumber/cucumber-expressions/](https://cucumber.io/docs/cucumber/cucumber-expressions/)

## 
**Page Object Model**


**Page Object Pattern**

Page Object Pattern also known as POM (Page Object Model) is a design pattern that define that per each screen there should be a corresponding page class. This Page class has the responsibility of finding all the elements as well as performing all the actions that belong to that screen.


## 
**Page Object Classes creation**

**Path:** Automation-UITests/src/test/java/com.company.test/pages

Each page object class must extends the base page **MobileBasePO**.

**MobileBasePO **class is responsible for creating the explicits waits. There are three different Wait Drivers:



*   waitDriver: it waits until the condition is meet for 15 seconds
*   `waitDriver = new WebDriverWait(driver, 15);`
*   waitDriverLong: it waits until the condition is meet for 70 seconds
*   `waitDriverLong = new WebDriverWait(driver, 70);`
*   waitDriverShort: it waits until the condition is meet for 2 seconds
*   `waitDriverShort = new WebDriverWait(driver, 2);`

_Wait Drivers - Explicit Waits_

The explicit wait is used to tell the WebDriverWait to wait for certain conditions (_Expected Conditions_). WebDriverWait by default calls the ExpectedCondition every 500 milliseconds until it returns successfully, if not, then an exception is thrown. Example:


```
getWaitDriver().until(ExpectedConditions.elementToBeClickable(By.id("Signature Rice Plate"))).click();
```


**Page example**


```
public class CheckOutPage extends MobileBasePO {

String payNowId = "Pay now";
String emailPredicate = "name LIKE '*Email:*'";

public CheckOutPage(AppiumDriver driver) {
super(driver);
}

public void payOrder() {
getWaitDriver().until(ExpectedConditions.elementToBeClickable(By.id(payNowId))).click();
}

public void tapEmail() {
getWaitDriver().until(ExpectedConditions.elementToBeClickable(MobileBy.iOSNsPredicateString(emailPredicate))).click();
}

}
```



## 
**Locators Strategies **

There are multiple ways to find an element:


<table>
<tr>
<td><strong>Strategy</strong>
</td>
<td><strong>Description</strong>
</td>
</tr>
<tr>
<td>Accessibility ID
</td>
<td>Read a unique identifier for a UI element. For XCUITest it is the element's <code>accessibility-id</code> attribute. For Android it is the element's <code>content-desc</code> attribute.
</td>
</tr>
<tr>
<td>Class name
</td>
<td>For IOS it is the full name of the XCUI element and begins with XCUIElementType. For Android it is the full name of the UIAutomator2 class (e.g.: android.widget.TextView)
</td>
</tr>
<tr>
<td>ID
</td>
<td>Native element identifier. <code>resource-id</code> for android; <code>name</code> for iOS.
</td>
</tr>
<tr>
<td>Name
</td>
<td>Name of element
</td>
</tr>
<tr>
<td>XPath
</td>
<td>Search the app XML source using xpath (not recommended, has performance issues)
</td>
</tr>
<tr>
<td>Image
</td>
<td>Locate an element by matching it with a base 64 encoded image file
</td>
</tr>
</table>


IDs strategies are the most appropriate. 

Examples:

By.id. \
`getWaitDriver().until(ExpectedConditions.elementToBeClickable(By.id("Signature Rice Plate"))).click();`

By.className.


```
getWaitDriver().until(ExpectedConditions.presenceOfElementLocated(By.className("XCUIElementTypeCollectionView")));
```


By coordinates through TouchAction.


```
TouchAction goToCart = new TouchAction(getDriver());
goToCart.tap(point(940, 40));
goToCart.perform();
```


By.xpath. It’s the less performant, try not to use it.


```
getWaitDriver().until(ExpectedConditions.elementToBeClickable(By.xpath("//XCUIElementTypeApplication[@name=\"Kiosk\"]/XCUIElementTypeWindow[1]/XCUIElementTypeOther/XCUIElementTypeOther/XCUIElementTypeOther/XCUIElementTypeOther/XCUIElementTypeOther/XCUIElementTypeOther[1]")));
```


There is one additional strategy which is not in the above table. It’s By Predicate. It’s a very useful method for when the Name attribute is partially dynamic. 


```
String addButtonPredicate = "name LIKE '*Add |*'";

getWaitDriver().until(ExpectedConditions.elementToBeClickable(MobileBy.iOSNsPredicateString(addButtonPredicate))).click();


<!-- Docs to Markdown version 1.0β17 -->

