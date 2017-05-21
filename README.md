# eurekaclinical-parent-cas
[Atlanta Clinical and Translational Science Institute (ACTSI)](http://www.actsi.org), [Emory University](http://www.emory.edu), Atlanta, GA

# What does it do?
It is a parent pom for CAS-related projects. It depends on the [eurekaclinical-parent](https://github.com/eurekaclinical/eurekaclinical-parent) organization pom. It specifies versions of all of the JASIG CAS server packages in the `dependencyManagement` section. If you use this as a parent pom, you still need to specify the dependencies that you need in your dependencies section.

Here are the packages and what they do:

* Core packages
  * `cas-server-core`
  * `cas-server-webapp`
  * `jstl`
  * `commons-pool`
  * `cas-server-support-trusted`

* Using a database to checking usernames and passwords
  * `cas-server-support-jdbc`

* Using the REST APIs for login and logout
  * `cas-server-integration-restlet`
  
* Connecting to an LDAP directory to check usernames and passwords
  * `cas-server-support-ldap`
  * `spring-security-ldap`
  
* Delegating authentication to an OAuth provider
  * `cas-server-support-oauth`
  


## Version history
### Version 1
Provides CAS server version 3.5.2.

## Requirements
* [Oracle Java JDK 8](http://www.oracle.com/technetwork/java/javase/overview/index.html)
* [Maven 3.2.5 or greater](https://maven.apache.org)

## Specifying this pom as a parent
```
<parent>
    <groupId>org.eurekaclinical</groupId>
    <artifactId>eurekaclinical-parent-cas</artifactId>
    <version>version</version>
</parent>
```

## Getting help
Feel free to contact us at help@eurekaclinical.org.
