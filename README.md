# Console-Based-Library-Management-System-LMS-
The Console-Based Library Management System (LMS) is a console-based Java application designed to facilitate the management of a library's resources and operations. This documentation outlines the features, architecture, and functionalities of the system. This system is based on MVC Architecture.
# Console-Based Library Management System

## 1. Introduction
The Console-Based Library Management System (LMS) is a console-based Java application designed to facilitate the management of a library's resources and operations. This documentation outlines the features, architecture, and functionalities of the system. The system is based on MVC Architecture.

## 2. Objective
The primary objective of the Library Management System is to provide a user-friendly and efficient platform for users to access and utilize these resources effectively. Specifically, the operations include add book, get book, remove book, and update book.

### Library Setup
During application startup, the librarian enters the library's name, address, and pin code, which are stored for future reference.

### Book Management
- **Add Book:** The librarian can add new books to the library by providing details like book name, author, and price.
- **Remove Book:** The librarian can remove books from the library by entering the book name.
- **Update Book:** The librarian can update existing book information (name, author, or price) by searching for the book and then modifying the desired field.
- **Get Book:** The librarian can search for a book by name and view its details (name, author, price).

## 3. Understanding MVC Architecture

### 1. Introduction
Model-View-Controller (MVC) is a software architectural pattern commonly used in the development of user interfaces, particularly web applications. It separates the application into three interconnected components, each responsible for a specific aspect of the application's functionality.

### 2. Components of MVC:
- **Model:** Represents the application's data and business logic. It encapsulates the data and defines how it can be accessed and manipulated. The model notifies the controller of any changes to its state, allowing the controller to update the view accordingly.
- **View:** Represents the presentation layer of the application. It displays the data provided by the model to the user and handles user interactions. The view receives input from the user and sends it to the controller for processing.
- **Controller:** Acts as an intermediary between the model and the view. It receives input from the view, processes it using the appropriate logic defined in the model, and updates the view with the results. The controller also listens for events triggered by the model and updates the view accordingly.
  
![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/bdf11f33-0311-47b3-8204-a8fed65652d6)

## 4. Details about Library Management System (LMS)

### Library Class:
- **Package Name:** `com.jsp.lms.model`
### Attributes (Fields):
1. `libraryName` (Type: String)
2. `libraryAddress` (Type: String)
3. `pincode` (Type: int)
4. `books` (Type: List<Book>)
### Methods:
- `getLibraryName()`: Returns the libraryName.
- `setLibraryName(String libraryName)`: Sets the libraryName.
- `getLibraryAddress()`: Returns the libraryAddress.
- `setLibraryAddress(String libraryAddress)`: Sets the libraryAddress.
- `getPincode()`: Returns the pincode.
- `setPincode(int pincode)`: Sets the pincode.
- `getBooks()`: Returns the books.
- `setBooks(List<Book> books)`: Sets the books.

### Book Class:
- **Package Name:** `com.jsp.lms.model`
### Attributes (Fields):
1. `bookName` (Type: String)
2. `bookAuthor` (Type: String)
3. `bookPrice` (Type: double)
### Methods:
- `getBookName()`: Returns the bookName.
- `setBookName(String bookName)`: Sets the bookName.
- `getBookAuthor()`: Returns the bookAuthor.
- `setBookAuthor(String bookAuthor)`: Sets the bookAuthor.
- `getBookPrice()`: Returns the bookPrice.
- `setBookPrice(double bookPrice)`: Sets the bookPrice.
- `toString()`: Overrides the toString method.

### View Class:
- **Package Name:** `com.jsp.lms.view`
### Attributes (Fields):
1. `library` (Type: Library)
2. `myInput` (Type: Scanner)
3. `controller` (Type: Controller)
### Methods:
- `getLibrary()`: Returns the library.
- `setLibrary(Library library)`: Sets the library.
- `main(String[] args)`: The main method containing program logic.

### Controller Class:
- **Package Name:** `com.jsp.lms.controller`
### Attributes (Fields):
1. `library` (Type: Library)
### Methods:
- `addBook(Book book)`: Adds a book to the library.
- `getBook(String bookName)`: Retrieves a book from the library.
- `update(Book bookExist, Book bookUpdate)`: Updates book details.
- `removeBook(String bookName)`: Removes a book from the library.

### List Interface:
- Used by the Library class to store books (`List<Book> books`).
- This is an interface implemented by various concrete list classes like ArrayList (likely used here).
- It provides functionalities for adding, removing, and accessing elements in a sequential order.

### One-to-Many Relationship (Library and Book):
- A single Library object can have a collection of many Book objects.
- This is reflected by the `List<Book> books` field within the Library class.
- The books list stores references to individual Book objects, each representing a book in the library.
## 5. Console-Based Library Management System Output

### Menu Options:
1. **Add Book**

 ![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/288ec088-15bd-49eb-b05c-e254a09f638d)

2. **Remove Book**

![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/57266a4c-5a43-42e4-a2d0-c702bde15e15)

3. **Update Book**

![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/2d8cad57-af67-4084-8979-6e0a420fada9)

4. **Get Book**

![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/ed143e14-0db2-4be3-9df0-c993b4ae4b58)

0. **Exit**

![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/c567fcf8-9539-40d6-a510-14bdf455ed87)


## 6.Flowchart for the Console-Based Library Management System:


![image](https://github.com/AditiShrivastav27/Console-Based-Library-Management-System-LMS-/assets/161911120/65fbf961-c2dc-4de5-8e88-f97384ef7c82)

