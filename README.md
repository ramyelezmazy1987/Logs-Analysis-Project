# Logs-Analysis-Project
### by Ramy Elezmazy

Logs Analysis Project, part of the Udacity
[Full Stack Web Developer Nanodegree](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd004).

## Project purpose
To write SQL queries to answer the following questions about a PostgreSQL
database containing the logs of a fictional newspaper website.

1. What are the most popular three articles of all time?
2. Who are the most popular article authors of all time?
3. On which days did more than 1% of requests lead to errors?


## Project contents
This project consists of the following files:

* `log_analysis.py` - The Python program that connects to the PostgreSQL
  database, executes the SQL queries and displays the results.
* `newsdata.zip` - A zip file containing a file that populates the `news`
  PostgreSQL database.
* `README.md` - This read me file.

## installation
This project makes use of the same Linux-based virtual machine
* Vagrant: https://www.vagrantup.com/downloads.html
* Virtual Machine: https://www.virtualbox.org/wiki/Downloads
* Download a FSND virtual machine: https://github.com/udacity/fullstack-nanodegree-vm and probably you will find the file in your “Download” folder.

Once you get the above software installed, follow the following instructions:
1. you need to bring the virtual machine back online ```bash vagrant up ```.
2. Log into it with ```bash vagrant ssh ```.
3. You will need to unzip `newsdata.zip` file after downloading it. The file inside is called ```bash  newsdata.sql```. Put this file into the vagrant directory, which is shared with your virtual machine.
4. To load the data, `cd` into the vagrant directory and use the command ```bash psql -d news -f newsdata.sql```.
5. Run ```bash python `log_analysis.py``` to answers to the three questions should now be displayed.

