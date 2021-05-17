# javaee-fundamentals


mvn clean package

java -jar ~/Downloads/payara-micro-5.2021.3.jar --deploy ./target/cdi-course-1.0-SNAPSHOT.war --port 8080

# JPA 
Mybatis does not implement JPA. Mybatis is not ORM Framework. JPA is ORM Specification which is implemented by Hibernate, Toplink, Eclipselink . Since Mybatis does not mplement JPA, it does not come under the list of JPA providers. Hence, you cannot use mybatis as a JPA framework. Mybatis is a data mapper framework which is completely different framework compared to JPA. In JPA and ORM frameworks, you map Objects /Entities to the corresponding sql tables and you work on objects and not on tables directly unless you use their native queries. In mybatis , you play directly with sql data.. Hope this clears the difference between mybatis and JPA. Hence when you want mybatis with spring data you use spring data mybatis independently and not spring data JPA.


# Scope
* Dependant means the scope of the bean is dependant on where it is injected
* RequestScope means that the (contextual)bean will be created when a new request comes and destroyed when a request finished
* SessionScope means the contextual instance will live throughtout a session
* ApplicationScope means the bean will live through the whole app life time(singleton)
* ConversationScope 