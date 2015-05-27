# Awesome Support Addon Boilerplate

This boilerplate is a starting point for creating addons for [Awesome Support](http://getawesomesupport.com). It contains all the things that are required in all addons, such as version checks and license activation.

The boilerplate should be used for all addons as it is uses a specific method to safely register itself with Awesome Support.

## Configuration

There is nothing much needed. Just rename the class and change the addon name. Here is the list of what needs to be changed:

- `AS_Boilerplate_Loader` (class name)
- `AS_Boilerplate_Loader::slug` (should be your addon name sanitized)
- `$plugin_name` in the `addon_license` method