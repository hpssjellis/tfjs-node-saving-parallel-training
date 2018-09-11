This node server allows saving individual layers so that multiple computers can work in parrallel to train a multilayer model
Sept 8, 2018 Still a work in progress but is basically working.

Note: I can't run this from github so people will have to load their own node server.

I made this on cloud 9 ( http:c9.io now absorbed by AWS) so not sure how it will work on your server.



On cloud nine use these steps. (On your machine you may have to place "sudo" infront of each step)

1. nvm install 8 (Only needed on cloud9 to insure using nodejs version 8 or above)
1. npm install
1. chmod 766 multi-layer-0.txt    (Set permissions on the data files so web users can write to the files)
1. chmod 766 multi-layer-1.txt 
1. chmod 766 multi-layer-2.txt 
1. chmod 766 multi-layer-3.txt 
1. edit the password and the URL inside the code
1. node multi-layer-server.js

1. (Load the webpage however that happens on your server. Hopefully you can click a link in the output from multi-layer-server.js)

Notes:   
-- Look at the multi-layer-server.js code, near the bottom of the page and change the password. Enter that password in the browser box and click "store info"

-- Look at the server code and change the URL (also near the bottom of the page). This must be your server URL for this file.

-- Presently the page is set to auto reload. Click pause to deselect auto so that you can have a look at how it works.

-- If your node server is private you may have to make it shareable.


![Also works on multiple computers](node-train.gif)



