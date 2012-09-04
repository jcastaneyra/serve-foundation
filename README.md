What is this?
=============

This is a simple HTML prototype written in HAML that is designed to be
viewed with Serve.

What is Serve? Serve is an open-source rapid prototyping framework for Web
applications. It makes it easy to prototype functionality without writing a
single line of backend code.


How do I install and run Serve?
-------------------------------

Serve is distributed as a Ruby gem to make it easy to get up and running. You
must have Ruby installed in order to download and use Serve. The Ruby download
page provides instructions for getting Ruby setup on different platforms:

<http://www.ruby-lang.org/en/downloads/>

After you have Ruby installed, open up the command prompt and type:

    gem install bundler

(OSX and Unix users may need to prefix the command with `sudo`.)

Then, run this command to install all dependencies:

    bundle install

After Serve is installed, you can start it up in a given directory like this:

    serve

This will start Serve on port 4000. You can now view the prototype in your
Web browser at this URL:

<http://localhost:4000>


Exporting
---------

To export your project, use the new "export" command:

    serve export <project>:<output>

Where "project" is the path to the project and "output" is the path to the
directory where you would like your HTML and CSS generated.


Learning More
-------------

You can learn more about Serve on the project page:

<http://get-serve.com>
