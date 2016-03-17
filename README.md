# html5-vidtest

This is a project to help illustrate some problems I am having with serving video to 
Safari, but not to other browsers, from WildFly. Tomcat works.  WildFly does not.

Build `./gradlew build`

Deploy the WAR build/libs/vidtest.war to WildFly

Open this URL in Chrome, Firefox and Safari: http://localhost:8080/vidtest/

You should be able to play the video in Chrome and Firefox, but not Safari.

<<<<<<< HEAD
Now deploy to Tomcat.  

You'll notice that you can view the video in all the browsers when served from WildFly.
=======
Now deploy to Tomcat.  You'll notice that you can view the video in all the browsers when served from Tomcat.
>>>>>>> bd15ad44b91a2305362f082518d144ad3b5673a2

