python-program-structure
========================

A simple Structure to start Python Applications

Installed / Dependencies
-------------------------------------------

This is just a simple structure for small applications (only used throught cli or module).

This structure is compatible with :
 * setuptools : the setup.py is working fine
 * py.test : all the unittest are in the /tests/ folder
 * sphinx : all the documentation are going to /docs/ folder

How to Use
-------------------------------------------

At any time you can build the app with

    python setup.py install

and your app will be accessible in your environment

    > myapp

I suggest you to look at the setup.py and changed some informations

How to Test it
-------------------------------------------

To test it, you will need py.test (you can install it with '''pip install -U pytest''')

    cd tests
    py.test

It will automatically run all the tests which are in the /tests/ folder

How to Generate the documentation
-------------------------------------------

To generate the documentation, I suggest you to use sphinx (you can install it with '''apt-get install python-sphinx''')
To build the doc generator, execute :

    sphinx-apidoc -F -o docs src

You can modify the '''docs/conf.py''' to match your need
And when you're ready, just go to the '''docs''' folder and run

    make html