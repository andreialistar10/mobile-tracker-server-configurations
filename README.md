# mobile-tracker-server-configurations
Configurations for mobile tracker server application

1. Microservices responsible for domain operations (<b>device-service</b>, <b>location-service</b>, <b>notification-service</b>, <b>user-service</b>) have configurations for development, production and test. For these, the structure is the following:

    - {application-name}/{profile}/{application-name}.yml
    where <b>profile</b> can be: <b>development</b>, <b>test</b> or <b>production</b>
    
2. <b>common-configurations</b> (such as liquibase, jpa, security, rabbitmq) is the directory for configurations that will be shared across multiple microservices

3. <b>gateway-service</b> contains <b>gateway-service.yml</b> that has gateway configurations.

3. <b>discovery-service</b> contains <b>discovery-service.yml</b> that has eureka service discovery configurations.
