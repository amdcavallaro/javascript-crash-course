### Beginner

This is a course designed for introducing JavaScript and Node.js as a platform for backend applications.

It assumes that you know basic concepts of (object oriented) programming but we will start from the beginner level and build up. 

So, the more programming experience, the better — but total newbies are also welcome, provided that they invest the required amount of time for self-learning.

The course is designed around open-source technologies, so a Unix-like system, Linux or MacOS is preferred. Git and Visual Studio Code will be our main tools, along with Node.js. Windows is not preferred, but if you absolutely have to live on Windows, you should have a working git and Node.js installation, and the rest will work.

In the end we expect to come up with a simple backend application that gets deployed with Docker and provides a REST API before a MongoDB datastore. This will not be an easy task, but we are committed to get every attendee on this level :)

Finally, this is a challenging, intensive, but fun and resourceful course. We will strive to do better each and every week. It won’t be a bed of roses, but it will provide immense learning opportunities.

We also have a dedicated Slack channel (#js-crash-course) in the [GDG Cloud Slack](http://slack.gdgcloud.com/) to help out the attendees with their assignments outside the class hours. An invite link to our Slack can be found in each of the meetup events.

During the meetings a group of volunteers will be around to answer your questions.
Additionally, all our volunteers are online on Slack to answer your questions, in addition to several online-only volunteers. You'll spot them easily - they have a red cross helmet emoji as part of their names.

Additionally, all talks are recorded and uploaded to YouTube. This is done with the purpose to help all those who want to take our course and can't attend one meeting (e.g. if you caught a cold) or any meeting (e.g.  if you have to babysit). If you will watch all talks, live or online, and present a satisfying final project - you will get the graduation certificate.

#### Submitting your activities

Add your exercise solution to this [spreadsheet](https://tinyurl.com/yy59zqnj).

#### Syllabus

###### Lecture 1: JavaScript & ES6 Fundamentals

An introduction on how JavaScript works and how to take advantage of the new ES6 syntax and features. In this session, we cover the basic programming paradigms in JavaScript, as well as topics like OOP and functional programming. We use the Chrome browser as a playground for an interactive session.

[Recorded talk from Berlin](https://youtu.be/xgzHW_WqYnM)
[Recorded talk from London - no audio](https://youtu.be/MP0wROOhyH8)

###### Lecture 2: Node.js Ecosystem & Basics

A fast dive into the Node.js ecosystem, detailing its working principles. A brief intro to its implementation and moving on to making use of and creating modules. Demonstration of the previous JavaScript and ES6 fundamentals, delving into the module pattern and several examples to familiarize with npm packages. We also talk about interacting with the file system. Useful tools like PM2 and nodemon are introduced in this session, as well as live debugging with Node.js. We use Visual Studio Code as the IDE of choice.

[Recorded talk from Berlin](https://youtu.be/MP0wROOhyH8)
[Recorded talk from London](https://www.youtube.com/watch?v=nYlSmXIVP1Y&feature=youtu.be)

Resources from the lesson:
slides Ola: https://gdgcloud.slack.com/files/UNB13G9QX/FNH11BGNL/copy_of_es6.pdf
slides Lorenzo: https://slides.com/robota/deck-3 (note that you can navigate both horizontally and vertically)
code Lorenzo:
   https://github.com/robota-x/gdg_lesson2/tree/pre-lesson (finished)
   https://github.com/robota-x/gdg_lesson2/commits/pre-lesson (each commit is a savepoint with a description, if you click through you can see the changes)
video: I've taken a quick look, it looks decent. I'm currently uploading it to a host
Further links - some contain exercises, you can treat reading the resources and doing the exercises as extra homework :stuck_out_tongue:
* markdown: https://www.markdowntutorial.com/ - a nice tutorial
* backticks: https://superuser.com/questions/254076/how-do-i-type-the-tick-and-backtick-characters-on-windows
* styleguides:
   https://github.com/airbnb/javascript - AirBnB's public and quite widely adopted styleguide for javascript. It's a long set of prescriptions
   https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode - a plugin for VS Code that will automatically format your JS according to a styleguide
stack overflow: https://stackoverflow.com/questions/tagged/node.js - if you google something code-relate, you'll probably end up here. Community-drive, usually high quality answers
* npm: https://www.npmjs.com/ - main page and search bar for useful packages
* package.json: https://nodesource.com/blog/the-basics-of-package-json-in-node-js-and-npm/ - decent article giving a wider overview of what package.json is
* chalk: https://github.com/chalk/chalk - the package we used during the lesson
* github: https://github.com/ - online storage/dashboard for your version-controlled code. Useful to share code, most open source projects have a presence here
* intro to git: https://guides.github.com/introduction/git-handbook/ - a nice intro to git (the most widely used version-control tool) and github
* gitignore explanation: (bonus, search online what you use a .gitignore file for and why it's useful)
* (even more things to do: what the recorded lesson from berlin, similar but slightly different than what we've done and it actually goes into Debugging)
Finally some quick notes about things I forgot to make explicit during the presentation:
* One of the things that propelled JS to being so widely used is that (for now) it is the only language that works both in the browser and on the computer. So while a developer can pick Python, PHP, Java, Go, Node.Js... to build a server, if you want logic in your web pages, you have to use JS.
This means that you need to only learn a single set of rules and syntax to be able to work both on the frontend and backend (this is ofc, a very simplified view).
* The previous points helps to expand the answer to the question 'why would I want Node'. If you want to host a website, or some APIs, or a game, you need code running on a computer listening for requests. You can use any language (and there are hundred with different strenghts), but Node lets you do that using Javascript.
* In my live coding I failed to make the connection from extracting our function to a file (that works for a local project) to npm. Npm, as other package managers, let you easily bundle your functionality in a package, and upload to a remote host. This mean that we can take our sayHi function, upload it to npm, and when we need to use it in a different project, do something like npm install sayHi (or the name we gave to the package)

###### Lecture 3: Promises and Async Programming

This session focuses on solving the challenges of asynchronous programming with certain constructs in Node.js — promises, async and await keywords. We discuss how each implementation enables a certain way of programming, and introduce a control flow library called async. We also touch upon streams and stream programming.

[Recorded talk from Berlin](https://youtu.be/RH_lwP-mjVM)

London:

From Lorenzo & Ola:
* A repo I started last year with some incremental examples on promises, I hope it could help if you're a beginner https://github.com/robota-x/gdg_lesson3 
- the examples are not using es6 features as it was initially built for another course. I've slightly tweaked it but the intended audience was somewhat different
- there is a 99_gdg_class.js file which has a worked example similar to what we've done during the class. I've added it as I went through those examples with some of you
- there is a 'homework.md' file. It has some basic exercises you could do if you're still unsure about promises
other things to research if you're curious:
* what is the 'utf-8' encoding you specified - this is a possible resource https://stackoverflow.com/questions/2241348/what-is-unicode-utf-8-utf-16
* what is 'callback hell' - this a wordy article but interesting https://www.freecodecamp.org/news/how-to-deal-with-nested-callbacks-and-avoid-callback-hell-1bc8dc4a2012/
* if you want to have some more 'practical' stuff to do but are short on ideas, https://javascript30.com/ is free and has a lot of follow-along videos with cute ideas
finally, some extra youtube videos that might act as intro for the next lesson (again, quite basic, good for beginners, I fished them out of old lessons)
* how the internet works https://www.youtube.com/watch?v=7_LPdttKXPc
* slightly more about protocols https://www.youtube.com/watch?v=eesqK59rhGA
* recap on node (plus a small http server built at the end!) https://www.youtube.com/watch?v=pU9Q6oiQNd0
* [bonus comedy link] if you need to remember/learn HTTP status codes: https://httpstatusdogs.com/ edit: and cats https://boingboing.net/2011/12/14/http-status-cats-by-girliemac.html


###### Lecture 4: HTTP APIs with Express.js

An introduction to web applications with the express framework and most popular packages including sessions and authentication, as well middleware implementations. We go into the details of HTTP and talk about RESTful APIs. We start implementing an example back-end application with express. We briefly talk about real-time capabilities with WebSockets.

[Recorded talk from Berlin](https://www.youtube.com/watch?v=ofQu4y-5v6c)

London:
videos of the class (link will change, this is a temp one but working):
* question aboud promises vs callbacks: https://lorenzomixedstuff.s3-eu-west-1.amazonaws.com/gdg_lesson_4_promise_vs_callback.mkv
* part one (slides): https://lorenzomixedstuff.s3-eu-west-1.amazonaws.com/gdg_lesson_4_pt1.mkv
* part two (coding): https://lorenzomixedstuff.s3-eu-west-1.amazonaws.com/gdg_lesson_4_pt2.mkv
links and extra notions that might be interesting:
* docs for express, our server framework (not the only one available!): https://expressjs.com/
* docs for fs-extra, the file system package used during the lesson: https://www.npmjs.com/package/fs-extra
* how the internet works in 5 minutes (again, since very few people saw it): https://www.youtube.com/watch?v=7_LPdttKXPc
* informative if a bit slow video on IPs and DNS: https://www.youtube.com/watch?v=mpQZVYPuDGU
* article that goes a bit more into details in the localhost concept: https://whatismyipaddress.com/localhost
* lesson 4 from berlin. Similar argument, but longer and has more advanced coding, good complement to what we've done during the class: https://www.youtube.com/watch?v=ofQu4y-5v6c
* page for pug: in the Berlin lesson some html templating is used, which I removed from the lesson due to time constrains. The idea is that you want to dynamically create/update the content of a page before sending it to the client. Rather than writing plain html, you use a custom language that then is compile into normal html5. https://github.com/pugjs/pug
* a quick blog on relational vs non-relational db (good for next lesson!). I think it's aimed at people with some knowledge around progarmming already. https://clockwise.software/blog/relational-vs-non-relational-databases-advantages-and-disadvantages/

###### Lecture 5: Adding a MongoDB Datastore

This session improves on the previous express application and introduces a MongoDB database as the datastore. We look into mongoose ODM and how to model simple data structures in MongoDB. We also talk about database denormalization approaches MongoDB enables. Further experiments with MongoDB queries and wiring the REST endpoints of the express app to real data.

[Recorded talk from Berlin](https://www.youtube.com/watch?v=EYYO4Le8bWQ)

###### Lecture 6: Testing

This session focuses on testing Node.js applications and the APIs that we have developed. We talk about general best practices in testing software, and several layers of application testing including unit testing, integration testing and acceptance testing. We implement several tests for our APIs with the test runner [AVA](https://github.com/avajs/ava).

[Recorded talk from Berlin](https://www.youtube.com/watch?v=NXMwf2OSVWQ)

###### Lecture 7: The Frontend

It’s time to give our application a real face. In this session we will go over the best practices of frontend engineering and building user interface applications. We will look at Vue.js, talk about its features and capabilities, and build a simple frontend with it.

[Recorded talk from Berlin](https://www.youtube.com/watch?v=io-hSpo_Yos&index=11&list=PL9pDl_Oth4cruQEVM4qUBKN-H4QMWGNNU)

###### Lecture 8: Deploying & Scaling Apps with Docker

The final session in this series introduces the final step in an application's lifecycle — the deployment. We learn the basics of Docker and how to deploy our Node.js applications with Docker. We introduce the concepts of continuous integration and continuous deployment, as well as automated testing. This session also includes scaling Node.js applications with load balancers and a reverse proxy setup with nginx.

[Recorded talk from Berlin](https://youtu.be/R2eYylz41Gg)

###### Lecture 9: Graduation Event

We will gather to see the final projects and cheer our classmates!

See the [graduation event pictures of the event in Berlin](https://www.facebook.com/pg/WomenTechmakersBerlinPage/photos/?tab=album&album_id=1561335890621986)

Last year, Women TechMakers Berlin had the talk "JavaScript is a Buffet, not a Main Course" by [Chris Heilamnn](http://christianheilmann.com/),

Talk Description:
Now that you learned about JavaScript, you're ready to take on the world as JavaScript runs everywhere. The trick is to not get overwhelmed and to find what makes you happy as happy developers are effective developers.

Chris Heilmann has a 18 year old history of using the language and wrote many books about it. Let him help you not get lost in the rabbit hole that is JavaScript in 2017.

Read about the talk: [So, you learned JavaScript – what now?](https://christianheilmann.com/2017/12/05/so-you-learned-javascript-what-now/)



#### How to join

Sign up on [Meetup.com](https://www.meetup.com/gdgcloud/events/263641541/).
Please be aware you'll be required to attend at least 80% of the classes to successfully complete the course.

#### Diversity and Code of 


Our mission is that everyone feels welcome to our events no matter gender or
nationality, take their first steps in tech and be part of our local community.

We don’t tolerate any kind of bad behaviour as defined by the [code of conduct](https://pastebin.com/Lez19E1N).

#### Location

Eurostaff Group Ltd

Newcomen St · London

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2483.5608396471985!2d-0.09138699999999998!3d51.502925999999995!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNTHCsDMwJzEwLjUiTiAwwrAwNScyOS4wIlc!5e0!3m2!1sen!2suk!4v1567578086500!5m2!1sen!2suk" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen=""></iframe>

#### Communication

Join the [GDG Cloud Slack](https://join.slack.com/t/womentechmakersberlin/shared_invite/enQtMjQ1ODcwNTIyMTAxLTY1NmVjMGQzOTgxNmI0ZWUwYWNlNDg0MjkyYjEwNDY5ZjVlMzU1ZDZlMjc1MGUzNzRhZWM3YzYxMDVmNWYzNjQ).

Join the #js-crash-course channel.

#### FAQ for Students

**Do I need to attend to all the sessions?**

We require at least attending at least 80% of the classes.

**Do I need to present a final project for graduation?**

Yes, presenting your project at the closing event is required to get the certificate of completion.

**I skipped some lessons and I am lost. Can I still come to the events?**

Ping the coaches on Slack, who can help you plan your catching up.

**How many hours do I need to study each week?**

Ideally you'll keep working on your project at home. We recommend investing about 3 hours a week in order to complete the whole course and do the project.

**Do I need to prepare the sessions at home?**

Yes, it is recommended that the students will review the recently taught material before each class.

**Who can attend?**

All genders are welcome.

**How do I RSVP for each lesson?**

RSVP opens for the next Meetup one week in advance, and you can RSVP during class.

**Will food be provided?**

There will be drinks and snacks.
