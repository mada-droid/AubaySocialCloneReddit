# Java Project

This repository contains a Java project that implements various functionalities for a social media platform. It includes configurations, controllers, DTOs, exceptions, mappers, models, repositories, security, and services.

## Project Structure

The project is organized as follows:

- **config**: This directory contains configuration classes used in the project. The following classes are included:
  - `SecurityConfig`: Configuration class for security-related settings.
  - `SwaggerConfiguration`: Configuration class for integrating Swagger API documentation.
  - `WebConfig`: Configuration class for web-related settings.

- **controller**: This directory contains controller classes responsible for handling API requests. The following classes are included:
  - `AuthenticationController`: Controller for authentication-related endpoints.
  - `CommentsController`: Controller for managing comments on posts.
  - `PostController`: Controller for managing posts.
  - `SubredditController`: Controller for managing subreddits.
  - `VoteController`: Controller for managing votes on posts.

- **dto**: This directory contains Data Transfer Object (DTO) classes used for data exchange between the client and server. The following classes are included:
  - `AuthenticationResponse`: DTO class for authentication response.
  - `CommentsDto`: DTO class for comments.
  - `LoginRequest`: DTO class for login requests.
  - `LogoutRequest`: DTO class for logout requests.
  - `PostRequest`: DTO class for creating posts.
  - `PostResponse`: DTO class for post responses.
  - `RefreshTokenRequest`: DTO class for refresh token requests.
  - `RegisterRequest`: DTO class for user registration requests.
  - `SubredditDto`: DTO class for subreddits.
  - `VoteDto`: DTO class for votes.

- **exceptions**: This directory contains custom exception classes used in the project. The following classes are included:
  - `PostNotFoundException`: Exception class thrown when a post is not found.
  - `SpringRedditException`: Generic exception class for the project.
  - `SubredditNotFoundException`: Exception class thrown when a subreddit is not found.

- **mapper**: This directory contains mapper classes responsible for mapping between different objects. The following classes are included:
  - `CommentMapper`: Mapper class for comments.
  - `PostMapper`: Mapper class for posts.
  - `SubredditMapper`: Mapper class for subreddits.

- **model**: This directory contains model classes representing different entities used in the project. The following classes are included:
  - `Comment`: Model class for comments on posts.
  - `NotificationEmail`: Model class for notification emails.
  - `Post`: Model class for posts.
  - `RefreshToken`: Model class for refresh tokens.
  - `Subreddit`: Model class for subreddits.
  - `User`: Model class for users.
  - `VerificationToken`: Model class for verification tokens.
  - `Vote`: Model class for votes on posts.
  - `VoteType`: Enumeration class representing different types of votes.

- **repository**: This directory contains repository interfaces responsible for database operations. The following classes are included:
  - `CommentRepository`: Repository interface for comments.
  - `PostRepo`: Repository interface for posts.
  - `RefreshTokenRepo`: Repository interface for refresh tokens.
  - `SubredditRepo`: Repository interface for subreddits.
  - `UserRepo`: Repository interface for users.
  - `VerificationTokenRepo`: Repository interface for verification tokens.
  - `VoteRepo`: Repository interface for votes.

- **security**: This directory contains security-related classes used in the project. The following class is included:
  - `JwtProvider`: Class for generating and validating JSON Web Tokens (JWT) for authentication and authorization.

- **service**: This directory contains service classes that handle the business logic of the application. The following classes are included:
  - `AuthenticationService`: Service class for authentication-related operations.
  - `CommentService`: Service class for managing comments on posts.
  - `MailContentBuilder`: Service class for building email content.
  - `MailService`: Service class for email-related operations.
  - `PostService`: Service class for managing posts.
  - `RefreshTokenService`: Service class for managing refresh tokens.
  - `SubredditService`: Service class for managing subreddits.
  - `UserDetailsServiceImpl`: Implementation of the `UserDetailsService` interface for Spring Security.
  - `VoteService`: Service class for managing votes on posts.

## How to Run

To run the project, follow these steps:

1. Clone the repository to your local machine.
2. Make sure you have Java Development Kit (JDK) installed.
3. Build the project using your preferred build tool (e.g., Maven or Gradle).
4. Run the application by executing the main class or using the build tool's run command.
5. Access the APIs using a REST client or web browser.

Please note that you may need to configure the project with your own database settings and other environment-specific configurations.

## Dependencies

The project has dependencieson the following libraries and frameworks:

- Spring Boot: A framework for building Java applications.
- Spring Security: Provides authentication and authorization capabilities for the application.
- Spring Data JPA: Simplifies database operations by providing a repository abstraction.
- Spring Web: Implements web-related features and RESTful APIs.
- MapStruct: A code generation library for object mapping.
- JSON Web Token (JWT): A library for generating and validating JWTs for authentication.
- Swagger: A library for generating API documentation.

Make sure to include these dependencies in your project's build configuration.

## Conclusion

This Java project provides a foundation for building a social media platform(Kinda of a clone to Reddit). It includes various components for handling authentication, managing posts and comments, interacting with subreddits, and more. Feel free to explore the different directories and classes to understand the project's structure and functionality.

If you have any questions or encounter any issues, please don't hesitate to contact me. Enjoy working with the project!
