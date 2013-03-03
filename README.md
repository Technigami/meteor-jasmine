space-daisy
===========

Jasmine standalone for Meteor apps. 
This is my first stab at putting something together for Jasmine with Meteor.
It uses a lot of symlinks. not sure yet how I feel about that but it works.

usage
-----

clone this repo and rename it for the project you want to test.
I have been using the naming convention yourProject-space-daisy

cd into yourProject-space-daisy and set up the symlinks

    cd yourProject-space-daisy
    ln -s path/to/yourProject src/yourProject
    ln -s src/yourProject/.meteor .meteor

put your jasmine specs in /specs and that should do it.
meteor will run SpecRunner.html which will run all your specs in the
context of the meteor app. Run meteor and check localhost:3000
