# Bootstrap - Salesforce

This is a simple fork of bootstrap to integrate a few changes to make it easier to work with in Salesforce. The only thing Salesforce specific is the ability to build to a .bundle (zipped resource for salesforce static resources). The other (current) change is to wrap every bootstrap class in a .bootstrap-enabled class so we don't clobber the surrounding markup or break any existing implementations when using Bootstrap.

## How to Use ##

If you want - just use the committed .bundle directory and upload to your static-resources.

## Building Custom Changes

If you want to make any changes to the source (e.g. change the wrapper template) make your changes to the .less files and then do the normal ```grunt dist``` task.  Then run ```grunt compress:salesforce``` to package as a new .bundle. It will be placed in the project base dir.

## Todos / Ideas ##
- Allow integration with Bower so we can include the scoped CSS in a Salesforce Seed App
- Add remote publshing of bundle to remote Salesforce project
