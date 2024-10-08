Developing Drools and jBPM
==========================

**If you want to build or contribute to a droolsjbpm project, [read this document](https://github.com/kiegroup/droolsjbpm-build-bootstrap/blob/master/README.md).**

**It will save you and us a lot of time by setting up your development environment correctly.**
It solves all known pitfalls that can disrupt your development.
It also describes all guidelines, tips and tricks.
If you want your pull requests (or patches) to be merged into master, please respect those guidelines.

# How to build with JBake

To build the drools-website (before and after your changes):

```
$ mvn clean generate-resources
```

## Local Build and Test

You can either use the JBake provided live-editing:

```
$ mvn clean jbake:inline
$ firefox http://localhost:8820
```

Alternatively, you may opt to generate the website with the standard Maven build, and then serve the content from your local FS:

```
$ mvn clean generate-resources && cd target/website && npx serve && cd ../..
$ firefox http://localhost:5000
```
