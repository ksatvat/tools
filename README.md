# Pyrhon Scanners & Tools


## Scan your code with Bandit and Snyk
An uncomplicated way to find security vulnerabilities and assess your Python security posture of your own Python code is to run a scan with Bandit.
Bandit is an open-source project that is available through the Python Packaging Index (PyPI). Bandit is a Python security tool that scans each .py file and builds a corresponding abstract syntax tree (AST). Bandit then runs several plugins against the AST to find common software security problems. For example, one plugin can detect whether you are using Flask (a micro-framework for Python) with the debug setting equal to True.
Bandit works either as a local tool to be used as you develop, or as part of your CI/CD (continuous integration/ continuous delivery) pipeline. You can create a YAML (Yet Another Markup Language) configuration file to control how Bandit behaves in these different scenarios. In this file you can also indicate a list of tests to skip. This functionality should be used with caution.
There is no guarantee that Bandit will catch all security problems—there are a finite number of plugins that it runs, and you could potentially have an issue in your code that does not register against any of the available plugins. However, it is one of those Python security tools that are easy to use and an excellent screen for common issues.

In 2021 Snyk added support for Python language. It provides security scanning on projects for vulnerabilities through our CLI and the application UI (app.snyk.io). Snyk allows you to automatically find, prioritize and fix vulnerabilities in your open-source dependencies throughout your development process.
In terms of dependency scanning, there are also other options like Requires, PyUp or Ochrona to scan and notify if there are any outdated packages.
