travel-blog-web
===============

Web portion of travel blog parse app


###Configuration###
Parse Cloud Code and Web Apps require a global.json
configuration file.  This file has been removed from the
repository for security reasons but it should look
exactly like this

````json
  {
      "applications": {
          "Travel Blog": {
              "applicationId": "APPLICATION_KEY", 
              "masterKey": "MASTER_KEY"
          }, 
          "_default": {
              "link": "Travel Blog"
          }
      }, 
      "global": {
          "parseVersion": "1.2.8"
      }
  }
````
Where APPLICATION_KEY is the parse project application key and
MASTER_KEY is the parse project master key.

Create this file exactly as above, replacing the two keys, and place it
in the parse/config/ directly as 'global.json'.

###Installing Parse Command Line Tools###
This project is deployed using parse command line tools, this will probably be enough
````bash
    curl -s https://www.parse.com/downloads/cloud_code/installer.sh | sudo /bin/bash
````

But you can also [click here for installation instructions](https://www.parse.com/docs/cloud_code_guide#started-installing)

