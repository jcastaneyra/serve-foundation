What is this?
=============

This is a simple HTML prototype written in HAML that is designed to be
viewed with Serve.

What is Serve?
--------------

Serve is an open-source rapid prototyping framework for Web
applications. It makes it easy to prototype functionality without writing a
single line of backend code.


How do I install and run Serve?
-------------------------------

Serve is distributed as a Ruby gem to make it easy to get up and running. You
must have Ruby installed in order to download and use Serve. **If you are on OSX, Ruby is already installed. Jump to step 2**.

### 1. Install Ruby

The Ruby download page provides instructions for getting Ruby setup on different platforms:

<http://www.ruby-lang.org/en/downloads/>

### 2. Install bundler

After you have Ruby installed, open up the command prompt and type:

    sudo gem install bundler


### 3. Install all needed parts

Then, run this command to install all dependencies:

    bundle install

This will take some time, and might ask for your password once, but it should be pretty painless.

After Serve is installed, you can start it up in a given directory like this:

    serve

This will start Serve on port 4000. You can now view the prototype in your
Web browser at this URL:

<http://localhost:4000>

Pow
---

Running 'serve' every time you want to access your project on a browser gets tiring pretty soon. So, the preferred way of running your project is through [Pow](http://pow.cx).

I've included the 'powder' gem to make this easier. If you've never installed pow, you can do so by running:

    powder install

You only need to do this once. Pow will be available for all your serve project from now on.

Now you need to tell Pow about your app. You do this by running:

    powder link

You'll get a notice on your terminal with the URL you can use to access your project.


LiveReload
----------

If you want to use LiveReload, open a terminal in your project folder and run:

    bundle exec guard -i

Keep it running, and you'll have a system that refreshes your CSS without reloading the page if you edit anything on the 'sass' folder, and reloads the page if you change anything on the 'views' folder.


Exporting
---------

To export your project, use the new "export" command:

    serve export <project>:<output>

Where "project" is the path to the project and "output" is the path to the
directory where you would like your HTML and CSS generated.


Upgrading ZURB Foundation
-------------------------
If, for some reason, you feel the need to update the bundled Foundation version (say: I forget to upgrade the gem when a new version comes out :) follow these steps:

- bump the gem version for 'zurb-foundation' in `Gemfile`
- run `bundle install` to install the new version (and all dependencies)
- run `rake upgrade` to update the files in the public, sass and views folders (beware: if you've edited any of the files, you'll most probably lose your edits. The command is intended to be run on a clean repository clone).


Learning More
-------------

You can learn more about Serve on the project page:

<http://get-serve.com>
