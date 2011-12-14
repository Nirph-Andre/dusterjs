Duster.js - Node script to watch & compile directory of dust.js templates
==============

Install

    npm install dust
    npm install watch-tree

Usage

    $ node duster.js

All dust templates in src folder will be rendered to public folder (you can modify folder paths in duster.js)

For example:

    ./src/dusts/tweet.dust
    ./src/dusts/user.dust

Compiles to:

    ./public/dusts/tweet.js
    ./public/dusts/user.js

Then you include them in the html:

    <script src="dust-core-0.3.0.min.js"></script>
    <script src="tweet.js"></script>
    <script src="user.js"></script>

I then use Jammit to concatenate all the JS files before production deployment.

by Dan McGrady http://dmix.ca