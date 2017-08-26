# blanco-sfdc-partner-build
This is a simple project to build sfdc-partner.jar file from partner.wsdl.

This is almost same as below:

```xml
<dependency>
    <groupId>com.force.api</groupId>
    <artifactId>force-partner-api</artifactId>
    <version>40.0.0</version>
</dependency>
```

## Usage

### Command

```sh
mvn antrun:run
```

### Input

```
./meta/partner.wsdl
```

### Output

```
./target/sfdc-partner.jar
```

## Purpose

sfdc-partner.jar will be used to access SFDC from Java with general object access.

You can get partner.wsdl from SFDC.

1. Access login.salesforce.com and login.
2. Open 'API WSDL'
3. Click 'Partner WSDL'
4. Click 'Generate Partner WSDL'
5. File => Save as : partner.wsdl
6. Put partner.wsdl into meta directory.
