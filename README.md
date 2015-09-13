## Simple Rails on on MySQL

#### Installing MySQL  
Enter in the terminal to install mysql on your machine
 ```$ brew install mysql```
### Controlling the server from the CLI
#### Starting the server
 ```$mysql.server start```

#### Stopping the server
  ```$mysql.server stop```

#### Getting the status of the server
 ```$mysql.server status```

#### Running mysql
 ```mysql -u root```
 gets you to a mysql prompt similar to typing ```psql``` to enter the postgres command prompt.

#### Exit out of the mysql command prompt by typing.
```exit```

#### Creating an app that uses mySQL as it's database
```rails new appname -d mysql```

#### Securing mySQL with a root password type
 ```mysqladmin -u root password```
 This tells mysql that you want to set an initial password. You will be prompted to enter a new password. If you had a password set previously, you would pass in the -p option and it will ask you for the old password then the new password.

#### To log in with your newly created password type
 ```mysql -u root -p```
 The p option tells mysql that you want to enter a password.

#### Installing the mysql ruby gem
 ```gem install mysql2```
 The 2 is a version made by someone else is listed as better...revision: in order to get this working properly on rails 4.2.1, you must specify an older version of the gem by typing ```gem 'mysql2', '0.3.18'```


#### Starting a rails app from a different port
```rails server -p 3001```
starts rails on port 3001
