#!/bin/bash

clear 

echo
echo "Working..."
echo

FILENAME=`basename "$1"`
CLEANNAME=`echo ${FILENAME// /_}`
FILEPATH=`echo ${1// /\\ }`

if [ -f "$FILEPATH" ]; then

        cp "$FILEPATH" /tmp/$CLEANNAME
        chmod 644 /tmp/$CLEANNAME
        `scp /tmp/$CLEANNAME "user@example_server.com:/path/to/accessible/folder/$CLEANNAME"`
        `rm -f /tmp/$CLEANNAME`
        URL="http://example_server.com/path/to/accessible/folder/$CLEANNAME"
        echo
        echo     "URL is:"
        echo
        echo "$URL"
        `/bin/echo -n "$URL" | pbcopy`
        echo
        exit 0

else
        sleep 1
        echo "Bad file path, try again."
        echo
        exit 1

fi
