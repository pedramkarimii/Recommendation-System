# Book Recommendation System

## Overview

The Book Recommendation System is designed to offer personalized book recommendations based on user ratings. Users can
view a list of books, rate them, and receive tailored recommendations based on their past ratings. The system utilizes
Django RESTful API, PostgreSQL, Redis, Docker, and Poetry for efficient management and deployment. The API documentation
offers details on how to use these endpoints, including request formats, response formats, and interactive testing.

## Features

- **User Authentication**: Secure access to APIs with email authentication.
- **Book Management**: View a list of books, their details, and filter by genre.
- **Rating System**: Users can rate books from 1 to 5, modify or delete their ratings.
- **Recommendations**:
    - **Based on Genre**: Suggest books in different genres based on previous ratings.
    - **Similar Users**: Recommend books highly rated by users with similar rating profiles.
    - **Insufficient Data**: Notify users if there's not enough data to provide recommendations.

## Technologies Used

- **Backend**: Django RESTful API
- **Database**: PostgreSQL
- **Cache**: Redis
- **Containerization**: Docker
- **Dependency Management**: Poetry
- **Testing**: Django TestCase
- **Scripting**: Bash scripts for setup and deployment
- **Email Authentication**: Integrated email-based user authentication

## Entity-Relationship Diagram for NetBaan

![ERD](ERD/ERD_NetBaan.pdf)

## API Documentation

The API documentation is available through the following interactive interfaces:

- **ReDoc**: Provides a user-friendly interface for exploring the API endpoints and their details.
- **Swagger UI**: Allows you to interact with the API directly from your browser, testing endpoints and viewing
  responses.

### Accessing API Documentation

Ensure that your Django server is running. You can access the API documentation at the following URLs:

- **API Schema**: [http://localhost:8000/schema/](http://localhost:8000/schema/)
    - This endpoint provides the raw OpenAPI schema for the API, which can be used for various tools and integrations.

- **ReDoc**: [http://localhost:8000/schema/redoc/](http://localhost:8000/schema/redoc/)
    - ReDoc offers a comprehensive, interactive documentation view of the API endpoints. It displays details about each
      operation, parameters, and responses in a clean interface.

- **Swagger UI**: [http://localhost:8000/schema/swagger-ui/](http://localhost:8000/schema/swagger-ui/)
    - Swagger UI provides an interactive API explorer where you can test API endpoints, see request and response
      formats, and execute API calls directly.

## Installation

To set up and run the Book Recommendation System, follow these steps:

1. **Clone the Repository**

   Fork and clone the repository from GitHub:

   ```bash
   git clone https://github.com/pedramkarimii/NetBaan-Sharif.git

2. **Navigate to the Project Directory**

```
cd NetBaan-Sharif
```

3. **Install Dependenciesy**

```
poetry install

```

4. **Set Up the Environment**

```
cp .env.example .env
```

5. **Run**

```
./utility/bin/setup.sh
```

6. **Run Tests (Optional)**

```
poetry run python manage.py test
```

### Fork and Contribute

To contribute to the project, you can fork it and submit a pull request. Here’s how:

1. **Fork the repository from GitHub**: [Fork Repository](https://github.com/pedramkarimii/NetBaan-Sharif)

2. **Clone your forked repository**:

   ```bash
   git clone https://github.com/pedramkarimii/NetBaan-Sharif
   ```
3. **Navigate to the Project Directory**:

   ```bash
   cd NetBaan-Sharif
   ```
4. **Create a new branch for your changes**:

   ```bash
   git checkout -b my-feature-branch
   ```
5. **Make your changes and commit them**:

   ```bash
   git add .
   git commit -m "Description of your changes"
   ```
6. **Push your changes to your fork**:

   ```bash
   git push origin master
   ```

#### 7. Create a pull request on GitHub:

Go to your forked repository on GitHub and click the "New pull request" button. Follow the prompts to create a pull
request from your fork and branch to the original repository.

### Author

#### This project is developed and maintained by Pedram Karimi.