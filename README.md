Learn-ruby
==========

Learning Ruby

This repo is intended to document my experinces as a beginner to Ruby.

Itended to help Ruby beginners like me.

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

http://packages.ubuntu.com/lucid/libsqlite3-dev

Make sure to download lucid version of libsql package.

Now install libsqlite and libsqlite-dev.









