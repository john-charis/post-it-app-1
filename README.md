# PostIt

PostIt supports collaboration and helps build relationships by allowing users create groups of other users. Broadcast messages can be sent to all members of these groups at the same time.

Different levels of priority can be set, so that users get notifications that betray the importance of the broadcast message.


## Getting Started
 PostIt is hosted on heroku and can be accessed by following these links: 
        In development: https://postit-app-develop.herokuapp.com/

        Production:
        https://postit-app-prod.herokuapp.com/

To use backend api's alone, please use the following instructions. 
  - Download and install [Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en)
  - Make sure you have working internet
  - Use the Service Api's below with Postman (See how in: Using Postman, below)


### Service Api's:
  - [Register](https://postit-app-develop.herokuapp.com/user/signup): Uses username, email and password
  - [log-in](https://postit-app-develop.herokuapp.com/user/signin):
  Uses email and password
  - [Create group](https://postit-app-develop.herokuapp.com/group):
  Takes in the name of the group, user must be signed in
  - [Add a user to your group](https://postit-app-develop.herokuapp.com/group/:groupId/user):
  Uses the params of the url, unique group id must be present, and the user you intend to add.


### Using Postman:
 - Install [Postman]((https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en))
 - In the postman window, populate the url window with the Api you want to take for a test run.
 - For the Service Api's listed above, click on the dropdown by the right of the url window, change from get to post
 - Click on the body tab, select the radio button: x-www-form-urlencoded
 - Populate the request body with the appropriate key value pairs: 
      - register : keys - email, password, userName
      - sign in: keys - email, password
      - create group: keys - groupname
      - add user: keys - user Id


## Prerequisites
 This are what you need installed on your computer to use the application:

 - [chrome] (https://www.google.com/chrome/browser/desktop/) browser
 - [Postman]((https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en))

 #### for devs:
 - [Git]((https://git-for-windows.github.io/))
 - [node.js]((https://nodejs.org/en/download/))
        ``` npm install ``` will install all dependencies



## Built With

- [Git]((https://github.com/)) - Version Control
- [node.js]((https://nodejs.org/)) - Js Environment
- [express](https://expressjs.com/en/starter/installing.html) - Server side Js tool
- [eslint](http://eslint.org/) - Linter
- [babel](https://babeljs.io/) - Transpiler 
- [firebase](firebase.google.com) - Persistent Storage and Authentication
- [Heroku](www.heroku,com) - Hosting and Continuous Deployment


## Authors

* **Osayamen** - *Initial work* [OsayamenOsaretin](github.com/OsayamenOsaretin)



## Acknowledgments
* Andela Bootcamp Facilitators and BFAs
* Andela Bootcampers
* Developer community
* Family
* Friends