space-daisy
===========

Jasmine standalone for Meteor apps. 
This is my first stab at putting something together for Jasmine with Meteor.
It uses a lot of symlinks. not sure yet how I feel about that but it works.

This is a very early attempt at making this work. Please bring up any issues
or situations where this is less than universally fantastic.

usage
-----

clone this repo and name it for the project you want to test.
I have been using the naming convention projectName-space-daisy

Set up the two symlinks then run meteor

    cd yourProject-space-daisy
    ln -s /path/to/yourProject src/yourProject
    ln -s src/yourProject/.meteor .meteor

Write some jasmine specs and put them in yourProject-space-daisy (or any folder
inside it other than lib) then run meteor.

    meteor

meteor will serve up main.SpecRunner.html on localhost:3000 which will run all 
your specs in the context of the meteor app. 
