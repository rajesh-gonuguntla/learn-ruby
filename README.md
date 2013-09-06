Learn-ruby
==========

Learning Ruby

This repo's intention is to document a beginer's experience & eamples on Ruby.


DAY 1:

Learning Objectives: 

1. Install Ruby Version Manager on my Ubuntu 12.04 LTS
2. Understand what RVM can do.


Install Ruby Version Manager on my Ubuntu 12.04 LTS
===================================================
Ref:  https://rvm.io/rvm/install#explained
      http://cheat.errtheblog.com/s/rvm
      
Ruby Version Manager allows you to easily install, manage, and work 
with multiple ruby environments from interpreters to sets of gems.


There are 3 ways to install RVM:

1. Single user
2. Multi User
3. Mixed

I've used multi user installation using the following command:

sudo curl -L https://get.rvm.io | bash -s stable

rvm release "rvm 1.22.3" was successfully installed on my ubuntu 12.04 LTS.


Install Ruby Dependencies using RVM
========================================
Now I tried to run "rvm requirements"

I was getting an error when I run rvm requirements
Error was something like this:
libsqlite3-dev: Depends: libsqlite3-0 (= 3.6.22-1) but 3.7.9-2ubuntu1 is installed

Solution for this is to remove ligsqlite3.7 manually and then installing libsqlite 3.6.22-1.
=>
http://packages.ubuntu.com/lucid/libsqlite3-dev
=>
Make sure to download lucid version of libsql package.
=>
Now install libsqlite and libsqlite-dev.
=>
Now run "rvm requirements" to install Ruby Dependencies.
=>
Install Ruby 1.9.3-p3392 by running the following command

"rvm install 1.9.3-p392"

Result is something like the following:
^Crajesh@ubuntu:~/Downloads$ rvm install 1.9.3-p392
Searching for binary rubies, this might take some time.
Checking requirements for ubuntu.
Requirements installation successful.
ruby-1.9.3-p392 - #configure
ruby-1.9.3-p392 - #download
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 11.3M  100 11.3M    0     0   589k      0  0:00:19  0:00:19 --:--:--  483k
ruby-1.9.3-p392 - #validate archive
ruby-1.9.3-p392 - #extract
ruby-1.9.3-p392 - #validate binary
ruby-1.9.3-p392 - #setup
Saving wrappers to '/home/rajesh/.rvm/wrappers/ruby-1.9.3-p392'........
ruby-1.9.3-p392 - #importing default gemsets, this may take time.......................









