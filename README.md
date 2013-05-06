Upload It!
-----------------

upload-it is a fun shell script that can be used as a kind of command-line replacement
for something like CloudApp on a Mac. The script will take any file you specify as an
argument, then upload it to your server for you.

Edit two things in the script:

1. On line 17, put the ssh username, url and correct file path for your webserver.

2. On line 19, edit the URL to reflect the publicly accessible URL for the path on your server.

Once you've got that done, make sure your SSH keys are set up, put the script somewhere in your
$PATH and make it executable.

Now when you want to share a file you can do:

	upload-it ~/Desktop/funnyimg.gif

...and the script uploads it for you, tells you the URL where you can find it, and puts that
URL on your clipboard so you're ready to paste it.


System Requirements
-----------------------

1. A Mac running a version of OS X that isn't from the Jurrasic era. 

2. Nothing else, really.