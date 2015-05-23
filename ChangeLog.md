# Versions #

## 0.5.0 ##
  * Exclude methods from JUnit 3 test case base classes from method proposals. [Issue 15 ](.md)
  * Support Groovy fixture template in New File dialog [Issue 3 ](.md)
  * There is now something vaguely resembling an UserManual
## 0.4.0 ##
  * Method proposals work for partial method names
  * Method proposals show type information and parameter names
  * Fix inherited fixture method completion and validation [Issue 1 ](.md)
  * Change fixture class loading from folder to project scope to find fixtures in another source folder [Issue 2 ](.md)
  * Check method exists for methods with parameters [Issue 13 ](.md)
  * New File dialog creating a Specification and a Java Fixture
## 0.3.0 ##
  * Validation if referenced fixture methods exist
  * Fixture method parameter count validation
  * First public release

## 0.2.0 ##
  * Syntax validations for all expressions
  * Code completion for partial namespace prefix should offer proposals not only for the prefix but for all available commands (e.g. `co|` -> `concordion:assertEquals`)

## 0.1.0 ##
  * Code completion for namespace prefix, commands, Fixture methods in expressions
  * Simple syntax validation for the `set` command
  * Recognizes Concordion Specs loaded in the HTML editor when the root element contains a declaration of a namespace prefix for the Concordion namespace (`http://www.concordion.org/2007/concordion`)

# Planned Features #

Listed in the issue tracker as [Open Enhancements](http://code.google.com/p/concordion-eclipse/issues/list?can=2&q=Type%3DEnhancement+&colspec=ID+Type+Status+Priority+Milestone+Owner+Summary&cells=tiles).

## Further Ideas ##
Ideas not yet listed in the issue tracker
  1. Quick Fix: Wrap marked text into span with concordion command
  1. Generate fixture from HTML (generate referenced methods)
  1. Generate HTML from template for fixture
  1. Partial document validation support (ISourceValidator)