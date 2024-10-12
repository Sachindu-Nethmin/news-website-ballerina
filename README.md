<h1>Set up</h1>



Clone the project

    $ git clone https://

Add a new file named Config.toml in the /backend_server directory and add the following configurations for the MySQL server.
    
    host = "<Database Host>"
    port = <Database Port>
    user = <Username of MySQL user>
    password = <Password of MySQL user>
    database = <database name>

 Run the following SQL query to create a new database in the MySQL server.

    CREATE DATABASE <database name>;

Run the SQL scripts backend_server/resources/init-data.sql to create the tables and insert data into the tables in the MySQL database.

Open a new Terminal in the project path and run the Ballerina service

    $ cd news-website/backend_server
<br>
    
    $ bal run

Then open a new terminal in the project path and run the React service
    
    $ cd news-website/frontend_server
<br>
    
    $ npm run dev

   
