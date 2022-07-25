# H2 Database Installation

## Learning Goals

- Explain the H2 database.
- Install H2 database on your machine.

## What is an H2 Database?

The H2 database is an open-source relational database for the Java platform. It
requires very little configuration to set up which makes it a great choice for
testing apps and for learning concepts without worrying about database specific
configurations.

You will usually see two main ways for storing data in H2 databases:

1. **In-memory Storage:** data is stored in the RAM while H2 is running. All of
   the data is removed once H2 is closed.
2. **Local Drive Storage:** data is stored on a local drive such as HDDs, SSDs,
   SD cards.

## Install H2 Database

In this section, we will install an H2 database and log into it on a browser.
The default user name for the database is `sa` and there is usually no password.
If an empty password field doesn’t give you access, try using `sa` as the
password.

First, we need to install and run the H2 local server and then we can use a web
browser to access the GUI.

### Mac Instructions

1. Go to the [H2 Database homepage](http://h2database.com/html/main.html).
2. Download the “All Platforms” zip file.
3. Extract the zip file into a directory (usually extracted as an `H2`
   directory).
4. Open a Terminal and navigate to the `bin` directory in the extracted
   directory.
5. Add execution permission for the `h2.sh` file by running `chmod +x h2.sh`.
6. Run `./h2.sh` to start the H2 database.

### Windows Instructions

1. Go to the [H2 Database homepage](http://h2database.com/html/main.html).
2. Download the “All Platforms” zip file.
3. Extract the zip file into a directory (usually extracted as an `H2`
   directory).
4. Navigate to the `bin` directory in the extracted directory.
5. Run the `h2.bat` file to start the H2 database.

The above steps should have opened up your web browser on `localhost:8082` and
show a GUI for logging in. Put `sa` for the username and keep the password field
empty. Click on “connect” to access the database.

![H2 database login screen](https://curriculum-content.s3.amazonaws.com/java-spring-1/h2-database-login-screen.png)

![H2 database home screen](https://curriculum-content.s3.amazonaws.com/java-spring-1/h2-database-homescreen.png)

Whenever you’re accessing the database in your Java app, make sure that the
database is running in the terminal or command line.

## Conclusion

In this lesson we have set up and accessed an H2 database. In later lessons we
will learn how to configure our Java apps to interact with the database.
