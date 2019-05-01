This is a base project from which we will be building our application.

Developer Instructions
----------------------

1. Fork this project
    * Rename the forked project to something else

1. in the `build.gradle` file, change the `group` to something else.

1. Create a Jenkins pipeline to your project from: https://ci.train.chikli.com/blue
    * New Pipeline - follow the instructions provided there

1. Configure Github to notify Jenkins when a checkin occurs via Webhooks
    * In your project fork, 
      * Settings -> Webhooks
      * Add Webhook
        * Payload URL: https://ci.train.chikli.com/github-webhook/
        * application/json
      * Verify that you get a green checkmark at the bottom of the page


Building the project
--------------------

Ensure you have the latest JDK 1.8 installed. Old versions, i.e. 1.8.0_61 will *not* work.

Linux: `./gradlew clean build` 

Windows: `gradlew clean build` 
