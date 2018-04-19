# Awesome Support Addon Boilerplate

[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/Awesome-Support/Addon-Boilerplate/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/Awesome-Support/Addon-Boilerplate/?branch=master)

This boilerplate is a starting point for creating addons for [Awesome Support](http://getawesomesupport.com). It contains all the things that are required in all addons, such as version checks and license activation.

The boilerplate should be used for all addons as it is uses a specific method to safely register itself with Awesome Support.

## Configuration

There is nothing much needed. Just rename the class and change the addon name. There is a more extensive list of what could be changed directly at the top of the boilerplate.php file.

## Usage

Your code should be placed in the `load` method. The easiest approach is to have all your code in a separate file and include this file from the `load` method.

**Be aware**, the addons are loaded by Awesome Support on the `plugins_loaded` hook with priority `20`. This means that when hooking within the `load` method, you **MUST** hook on `plugins_loaded` with priority `21` or later.

### Change Log
-----------------------------------------------------------------------------------------
###### Version 2.0.0
New: Use new base extension class that is in version 5.x of Awesome Support core.
New: Include change log in this read me file
New: Include some instructions directly at the top of the main class file (boilerplate.php)

-----------------------------------------------------------------------------------------
###### Version 1.0.0
Fix: Updated minimum compatibility levels for some items
New: Implement option to Set item id 
New: Use core classes to display messages
New: Use product id for updates instead of name
Tweak: Move constants inside of class
Fix: Issues with installation subdirectory
Tweak: Update usage instructions
Fix: Styling issues and typos


-----------------------------------------------------------------------------------------
###### Version 1.0.0
Initial Commit

-----------------------------------------------------------------------------------------