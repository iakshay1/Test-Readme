# Test-Readme

### This README would normally document whatever steps are necessary to get the application up and running.

## Ruby Version: 

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

## Homebrew Installation:

> When we run brew install, Homebrew reads our package's Formula — an implementation of Ruby's abstract Formula class that provides package metadata and installation instructions — to create an executable from our source code and install it locally on our computer.

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

## RVM:

> RVM is a command-line tool which allows you to easily install, manage, and work with multiple ruby environments from interpreters to sets of gems.

1. To install ruby and rails go to <https://rvm.io/>.

2. Open cmd and type the below command to install ruby and rails.
```
\curl -sSL https://get.rvm.io | bash -s stable --rails
```
This command installs both ruby and rails in your machine.

3. To check the version of ruby and rails  installed in your machine use the below command.
```
ruby --version
```

```
rails --version
```

4. After installing ruby and rails type this command to install ruby version 2.7.2 to avoid Augment error.
```
rvm install ruby-2.7.2
```
5. After the installation is done make this ruby version as default and current by using the below code.
```
rvm --default use ruby-2.7.2
```
---

## Yarn:

> Yarn is a package manager for JavaScript. It is used by Rails to manage JavaScript dependencies.

1. to install yarn in your machine first you have to install node. Open cmd and type the below command to install node.

```
brew install node
```

2. Once brew is installed you can use the below command to insall yarn.
```
brew install yarn
```
---

## PostgreSQL

> PostgreSQL possesses robust feature sets including Multi-Version Concurrency Control (MVCC), point in time recovery, granular access controls, tablespaces, asynchronous replication, nested transactions, online/hot backups, a refined query planner/optimizer, and write ahead logging.

1. To install postgreSQL in your machine type the following command in your cmd.
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
 
4. For more information visit <https://wiki.postgresql.org/wiki/Homebrew>.

---

## Installing dependencies

After cloning the project in your local machine using cmd try bundle install.

If you get an error like `ruby-dep 1.5.0 requires ruby version 2.2.5,~>2.2, which is incompatible with the current version` then try deleting the `gemfile.lock` and run the below command.
```
bundle install
```
---

After bundle install if you get an error like `install mime magic 0.3.10` then run the below command 
```
brew install shared-mime-info
```
After this command try the below command again 
```
bundle install
```
now it should install all the gemfiles required to run this project

---

## Unit Testing

> The main objective of unit testing is to isolate written code to test and determine if it works as intended.

For beginning the unit test in your local machine open VsCode and go to the terminal and type the below command. But befor that check whether you have the below specified gems in the gem file.

```
gem 'json_expressions'
```

```
gem 'simplecov' 
```

```
gem 'webmock'  
```

If the above specified gems not present in the gem file add it and then run the bundle command 

```
bundle install
```

After Installing use the below command to run the rails test

```
rails test -e qa
```

After it completed running open the index.html file in the generated coverage folder to check the code coverage.

---

## Bastion Host

> A bastion host is a server whose purpose is to provide access to a private network from an external network, such as the Internet.

#### QA

1. To start the bastion host instance in QA environment login into your [jenkins](https://jenkins.dso.credavenue.io/login?from=%2F) select Onboarding -> Utilities -> start-stop-onboarding-bastion-instance then click on build with parameters from the left column and then specify the int environment to start a instance in QA.

2. Once the instance has been started got to AWS CAPL and log in into you int onboarding role.

3. Select EC2 in console home 

4. Then click on Instances(running).

5. Then search for the instance you started in the jenkins

6. click on connect to connect to the instance.

             
             
