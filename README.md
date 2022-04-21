# SEA8 - Spring Data JPA Quest 01 - Hibernate

## Challenge: The magic of Spring Data JPA

_Fork_ the following repository: https://github.com/WildCodeSchool/quest-spring-jpa-hibernate.

You are taking over the development of a Harry Potter fan site in order to add more functionality. As it stands, the site allows users to manage all of the characters described in the wizarding universe from the series, using _Spring Data JPA_.

You're going to have to create a new empty database *spring_jpa_quest*:

```SQL
CREATE DATABASE IF NOT EXISTS `spring_jpa_quest`;
```

The user is the same as the one in the other JDBC quests with an id _h4rryp0tt3r_ and the password _Horcrux4life_. It will be necessary to grant the user all permissions over the database *spring_jpa_quest*:

```SQL
GRANT ALL PRIVILEGES ON spring_jpa_quest.* TO 'h4rryp0tt3r'@'localhost';
```

**Be sure to check all the classes in the repository before starting the challenge!**

1. Add the necessary configuration for the use of _Spring Data JPA_ inside _application.properties_ in the folder _src/main/resources_
2. Test that the site is working correctly
3. Modify the entity called _School_ to add the code necessary to use it with _Spring Data JPA_
4. Modify the interface called _SchoolRepository_ in order to make a DAO that correctly implements _JpaRepository_
5. Modify SchoolController in order to retrieve an instance of SchoolRepository via dependency injection
6. Add the CRUD operators to _SchoolController_ in order to make it possible to manage a school.

## Validation criterias

- The project runs correctly using the required database and user.
- It is possible to create a school.
- It is possible to modify a school.
- It is possible to display a list of all schools.
- It is possible to delete a school.
- The class _School_ contains all the necessary code to make it an entity.
- The class _SchoolRepository_ implements _JpaRepository_ correctly.
- The class _SchoolController_ retrieves an instance of _SchoolRepository_ via dependency injection.
- The code is available on GitHub.
