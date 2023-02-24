# Test-Readme

### This README would normally document whatever steps are necessary to get the application up and running.

#### Ruby Version: 

1. Open Cmd and chage the directory to where the project resides. Use the below command to change the directory.
```
cd
```

2. Type bundle install to install the required gems mentiond in this project
```
bundle install
```

3. If the build is failed check the gemfile and then try to update the project to the current version. For more reference visit: <https://rubygems.org>.

4. If you dont have the specified ruby version to run the project we have to install it using rvm.


---

#### Homebrew Installation:

1. open cmd and copy the below command and press enter to install homebrew in your local machine.
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Wait for it to insall homebrew in your local machine.

3. After the installation completion you have to setup your path for home brew. Use the below command to set the path.
```
echo 'PATH="/usr/local/bin:$PATH"' >> ~/.bash_profile
```

4. Now to check the brew version installed in your machine use the below command.
```
brew --version
```
---

#### RVM:

1. To install ruby and rails go to <https://rvm.io/>.

2.open cmd and type the below command to install ruby and rails.
```
\curl -sSL https://get.rvm.io | bash -s stable --rails
```
This command installs both ruby and rails in your machine.

3.to check the version of ruby and rails  installed in your machine use the below command.
```
ruby --version
```

```
rails --version
```
---

#### Yarn:
1. to install yarn in your machine first you have to install node. Open cmd and type the below command to install node.

```
brew install node
```

2. Once brew is installed you can use the below command to insall yarn.
```
brew install yarn
```
---

#### PostgreSQL
1. To install postgreSQL in your machine type the following commands in your cmd.
```
brew install postgresql
```
This installs the command line console (psql) as well as a PostgreSQL server locally, so you can create your own databases locally if desired.

2. Run the below command to start the server
```
brew services start postgresql
```
3. If you want to connect and use it as your user run the following command
```
 psql postgres
 ```
4.For more information visit <https://wiki.postgresql.org/wiki/Homebrew>.
---

              
             
             
