In this config server repo every file is created with a certain purpose.

application.yml - common file for storing the common properties of all services.

address.yml - it has the properties related to address service.

employee.yml - it has properties related to employee service.

It is necessary to note that the name of service/app should match with the name of specific file (eg address.yml) created for stroring it's properties. Doesn't matter if 
name of app is in upper case and file is in lower case or vice versa because this process isn't CASE SENSITIVE.

Also the name of application.yml is the default name that Spring Cloud Config Server looks for , if u want to have a custom name then u have to add
profile:default,(custom-name) under cloud.config. tree of yml of specific service to let that service use that file.
