This is the backend part of our Grading System application

Steps to run this project:
1. Clone this project
2. Run `npm i` command in the terminal to download all the modules used in this project
3. Database used was postgres. If you have no postgres you must install it first to continue
4. After you have installed postgres you must add postgres to your system path and to do so:
    - Search for environment variables in your computer and select edit the system environment variables
    - Select Environment Variables
    - Select Path in System Variables and click Edit
    - Add the bin directory of where you installed Postgres then click OK
5. After you have installed postgres configure the `src/data-source.js` file to make connection to your pg database.
    - What do I modify in the data-source.js file?
            - The username and password. Enter the username and password you used in your postgres client.
6. You must then create the database in your postgres client in Visual Studio Code and to do so:
    - Open the terminal for Visual Studio Code
    - Navigate to the directory of the project
    - Type psql -U postgres
    - Type CREATE DATABASE grading_system;
7. Congratulations you can now use the backend part of the grading system. To run the back end:
    - Open the terminal for Visual Studio Code
    - Run `npm run dev` command
