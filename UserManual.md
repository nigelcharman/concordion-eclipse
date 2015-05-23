# Introduction #

First, install the plugin following the steps in InstallingPlugin.

The plugin supports writing [Concordion Specifications](http://www.concordion.org/Tutorial.html), and is an extension to Eclipse's HTML and Web Page editors. To use it, you need to
  * Make sure you edit the Specification in the Eclise HTML source editor, or the source tab in the Web Page Editor. This is usually the case when you just doubleclick on a HTML file in an Eclipse installation with default configuration.
  * Declare a namespace prefix for the Concordion namespace on the HTML root element

```
  <html xmlns:concordion="http://www.concordion.org/2007/concordion">
    Test some <span concordion:assertEuals="getResult()">value</span>
  </html>
```

# New File Wizard #

Select the package where you'd like to have the Specification created in. Go to `File > New > Other...` to open the New File dialog. In the dialog, select `Concordion Specification with Fixture`:

![http://concordion-eclipse.googlecode.com/svn/trunk/doc/newfile.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/newfile.png)

A wizard page will appear. Change or set the location if desired, enter a name for the Specification (e.g. `CanOrderIceCream.html`) and select wether you'd like to generate a Java or a Groovy fixture to go with it.

![http://concordion-eclipse.googlecode.com/svn/trunk/doc/newfilewizard.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/newfilewizard.png)

# Code Completion #

To use code completion, hit Ctrl+Space (or whatever your code completion hotkey is) in any of the following places while writing the Specification:

## Commands ##
![http://concordion-eclipse.googlecode.com/svn/trunk/doc/commandcompletion.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/commandcompletion.png)

## Partial Namespace Prefix ##

![http://concordion-eclipse.googlecode.com/svn/trunk/doc/prefixcompeletion.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/prefixcompeletion.png)

## Fixture Methods ##
![http://concordion-eclipse.googlecode.com/svn/trunk/doc/methodcompletion.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/methodcompletion.png)

![http://concordion-eclipse.googlecode.com/svn/trunk/doc/methodcompletionprefix.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/methodcompletionprefix.png)

The list of methods will exclude:
  * Methods annotated with `@Before`, `@After`, `@BeforeClass`, `@AfterClass`
  * Methods from `Object`, `TestCase`, `ConcordionTestCase`
  * For JUnit3 fixtures, `setUp()`, `tearDown()`
  * Any methods not accessible from the fixture class

# Validation #

Vslidation is done automatically when you open a Concordion Specification in the editor, and as you type. Errors are marked with a red underlining, details are shown if you hover the mouse over the error.

## Command Name ##
![http://concordion-eclipse.googlecode.com/svn/trunk/doc/unknowncommand.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/unknowncommand.png)

## Expression Syntax ##
![http://concordion-eclipse.googlecode.com/svn/trunk/doc/expressionvalidation.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/expressionvalidation.png)

## Method Name ##
![http://concordion-eclipse.googlecode.com/svn/trunk/doc/methodvalidation.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/methodvalidation.png)

## Method Parameter Count ##
![http://concordion-eclipse.googlecode.com/svn/trunk/doc/paramvalidation.png](http://concordion-eclipse.googlecode.com/svn/trunk/doc/paramvalidation.png)