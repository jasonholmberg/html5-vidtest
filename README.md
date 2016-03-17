# html5-vidtest

This is a project to help illustrate some problems I am having with serving video to 
Safari, but not to other browsers, from WildFly. Tomcat works.  WildFly does not.

After cloning this project....

## Deploying to WildFly
The easiest way to do this is to deploy this app as an exploded war. 

1. `cd` to `<your-wildfly-install>/standalone/deployments`
1. Create a symlink to this project directory with the name `vidtest.war` kind of like this `ln -s ~/myprojects/html5-vidtest/ vidtest.war`
1. `touch vidtest.war.dodeploy` 

Now start WildFly, if it is not already running.

Open this URL in Chrome, Firefox and Safari: http://localhost:8080/vidtest/

You should be able to play the video in Chrome and Firefox, but not Safari.

Now deploy to Tomcat.  You'll notice that you can view the video in all the browsers when served from Tomcat.

