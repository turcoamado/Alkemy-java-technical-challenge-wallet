# ALKEMY JAVA TECHNICAL CHALLENGE - WALLET

### PROJECT SETUP & TOOLS
1. JDK 17
2. [MySQL](https://dev.mysql.com/doc/refman/8.0/en/installing.html).
3. [Postman](https://www.postman.com/downloads/) for testing endpoints.

### CODE STANDARDS
- Keep in mind rules from [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html).
- Code must be in English.
- The controllers should finish with suffix "Controller". Example: UserController.
- The services should finish with suffix "Service". Example: UserService.
- The repositories should finish with suffix "Repository". Example: UserRepository.
- The interfaces should start with prefix "I". Example: IUserRepository.
- The implementations should finish with suffix "Impl". Example: UserServiceImpl.
- The DTOs should finish with suffix "Dto". Example: UserDto, UserRequestDto.
- Usage of DTOs is a must. Can have DTOs for request and response.
- Package names are in singular.
- The names of attributes/fields from Java classes must be written using camel case. Example: firstName.
- The name of columns in the entities must be written using underscore and uppercase. Example: FIRST_NAME.The name of the tables is always in plural, but the entity name should be in singular.
- Exceptions should be handled by an implementation of ControllerAdvice. 
- Messages to user can't be hardcoded them should be handled. Some refs [here](https://looksok.wordpress.com/2014/07/05/string-externalization-in-spring-3-1-with-messagesource-no-web-xml/) and [here](https://zetcode.com/spring/messagesource/). 
- If you add a new endpoint, make sure to set the role access for it in the SecurityConfig class.


You will find an example of how to work with the project architecture in architecture-example branch.

### GIT STANDARDS

#### FORMAT
- Always create the branch from develop
- The branch name format is: `feature/{jiraTicket#}`.
- The pull request title format is: `{jiraTicket#}: {jiraTitle}`.
- The commits format is: `{jiraTicket#}: {commitDescription}`. Small commits are a nice to have.
- The pull request has to contain only the changes related to the scope defined in the ticket.
- Pull request should always be from your current branch to develop.

#### EVIDENCE
- If you do not write unit test or integration test as part of your code changes, you should add the HTTP request and response as evidence that the code is working as expected.
- Screenshots from Postman with different scenarios are a good way to show your work.

### RUN LOCALLY
On the root folder run:
```
mvn spring-boot:run
```