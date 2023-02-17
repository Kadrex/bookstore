# Bookstore

## Setting up Spring Boot application.

1. Make sure you have installed Java. For development OpenJDK 11 from [AdoptOpenJDK](https://adoptopenjdk.net/) should be used.
2. Install Intellij IDEA Commmunity edition
3. Import the Maven project
4. Run the LibraryApplication from IDE.

However, you can also install Maven and run the back-end from terminal with
`mvn spring-boot:run` in project directory
(make sure your JAVA_HOME variable is set up to point to
your Java 11 installation in that case)

## Setting up Angular application.

To get Angular app up and running you need to:

1. Make sure you have [NodeJS](https://nodejs.org/en/download/) version 10+ installed.
2. Open the terminal.
3. Navigate to frontend project `cd frontend/`
4. Install all dependencies with npm `npm install`. NB: This might take a while.
5. Start the development server `npm run start`.
   Frontend runs on port 4200, so make sure it's not in use.
   
   First build takes a lot of time, so be patient...

   ![Compiling](https://imgs.xkcd.com/comics/compiling.png)
6. Once development server is running, open app at http://localhost:4200. If you can see a list of books then it means that you have sucessfully set up and run the application


## Functionality

There are four main views: books view, checkouts view, favorite books view and late checkouts view. 
There are also individual views for books and checkouts and forms for adding a new book and checking out an existing book.

The four main views are accessible via menu on the left which opens up when the menu icon in the top left corner is clicked.

In books view user can see a table of books which can be filtered and sorted by every book parameter.
When user clicks on book, individual book view opens where the user can add the book to favorites, remove it from favorites or check it out.
If the user decides to check out the book and the book is available, checkout form appears.
In books view user can also find a button which takes it to a form to add a new book to the library.
In checkouts view user can see a table of checkouts which can be filtered by book parameters and borrower name.
If the user clicks on checkout from the table, individual checkout view appears and the user can return the book.

In favorite books view there are shown favorite books for current user. The user can remove books from favorites or check them out.

In late checkouts view user can see all the late checkouts. The user can return the books.
