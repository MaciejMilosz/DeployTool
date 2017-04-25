# DeployTool
Ant based tool for Salesforce deployment and validation



# How to use

Just copy the src folder, run console, and proper ant target. This can be easly used by developers to deploy code into dev orgs. JDK and Ant needs to be installed.

## Targets

* validatePackage used only to check if project is compileable
* validatePackageAndRunTests used to check if project is compilable and if all tests pass
* deployOnly used only to deploy project
* deployAndRunAllTests used to deploy project and run all tests in the org

## Properties

* sf.username: username which will be used by ant
* sf.password: password + security token
* sf.filesWithDeprecated: coma separated list of files with @deprecated in them (whole path)
* sf.filesWithNamespace: coma separated list of files with used namespace
* sf.version: API version to use
* sf.mainNamespace: main namespace used by the code (if is managed package code deployed to other org)
* sf.server: https://www.salesforce.com or for sandboxes: https://test.salesforce.com
