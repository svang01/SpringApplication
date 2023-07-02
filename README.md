Spring Boot CRUD Application
- This is a simple application that provides a user interface where you can add, edit, and delete books and authors. It utilizes a few technologies listed below to handle the backend operations and presents the data on the web pages. You can test the CRUD operations by running the Spring Boot application, accessing it in your web browser, and performing the desired actions.

Technologies Used:
- Spring Boot
- Spring Web
- Thymeleaf
- Spring Data JPA

To run the application, follow these steps.
- Clone the repo
- Open project in preferred IDE (VS Code, Intellij, etc)
- Run the "Spring Application" class to start the spring boot application.
  - The Application will start running on http:localhost:8080
  - Either click on Add Authors or Add Books to get started

Functionality:
- Book Entity
  - Add Books 
    - Navigate to http://localhost:8080
    - Click "Add Books"
    - Enter the Title and Author and click "Add"
  - Edit 
    - Once the book is created, click on the "Edit" button on the book you want to modify.
    - Update the title or author details in the form and click update.
    - This page will update with your changes and also list all books in the directory.
  - Delete
    - Simply press the "Delete" button on the book and author you want to delete.
    - The page will update with the removal of the book and author you wanted to delete. 


- Author Entity
  - Add Authors
    - Navigate to http://localhost:8080
    - Click "Add Author"
    - Enter the Author and click "Add"
  - Edit
    - Once the author is created, click on the "Edit" button on the author you want to modify.
    - Update the author details in the form and click update.
    - This page will update with your changes and also list all Authors in the directory
  - Delete
    - Simply press the "Delete" button on author you want to delete.
    - The page will update with the removal of the author you wanted to delete.
    
Testing:
- To Test the CRUD Operation, follow these steps:
  - Start Spring Boot Application
  - Open your web browser and navigate to http://localhost:8080.
  - Click on either Add Authors or Add Books.
  - Create, Update, or Delete as desired.
  - Verify that the changes are reflected in the application.


Additional Information:
- Repository Package
  - This package contains interfaces that define the data access operation for the book and author entity.
  - Both interfaces extend the "JpaRepository" by which allowing the repositories to inherit various methods for performing CRUD operations. 
- Model Package
  - The model package contains data for the books and authors.
  - The book class contains properties such as 'id', 'title', and 'author'
  - The author class contains properties such as 'id', 'name', and 'books'
- Controller Package
  - This controller package contains classes that handles incoming request.
  - The book controller handles CRUD operations related to books.
  - The author controller handles CRUD operations related to authors.
  - The controllers are annotated with @controller to indicate they are responsible for handling http requests. In addition, the @requestmapping defines the base path for their respective functionalities.