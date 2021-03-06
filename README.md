# Harry Potter Statistics Project - Code Academy Stream 2

You can view the project here: harry-potter-statistics.herokuapp.com


### Purpose and need of project

The project itself shows a variety of statistics related to the very popular book series 'Harry Potter'.
The purpose of the project is to show the user how many characters mentioned throughout the series meet 
the requirements set by the user. The user can easily find out, for example, how many characters were a
part of the 'Slytherin' House and were female. The application itself has a counter at the top that easily
displays the total amount of people that meet the specified criteria and the charts adjust as the user clicks
on them to portrait more data about the group of people shown by the number in the counter.


### Database Information

The database consists of information I collected off the following source:
* https://en.wikipedia.org/wiki/List_of_Harry_Potter_characters
* http://harrypotter.wikia.com/wiki/Main_Page

The Database CSV file is included.

The database is run through the Heroku application add on called mLab. The database was formatted in a csv file and
imported into a MongoDB database. 


### Technologies Used
Technology Name | Description
------------ | -------------
[Flask](http://flask.pocoo.org/) | Flask is a microframework for Python based on Werkzeug, Jinja 2 and good intentions.
[MongoDB](https://www.mongodb.com/) | Document-oriented (NoSQL) database using JSON-like documents.
[dc.js](https://dc-js.github.io/dc.js/) | dc.js is a javascript charting library with native crossfilter support, allowing highly efficient exploration on large multi-dimensional datasets (inspired by crossfilter's demo). It leverages d3 to render charts in CSS-friendly SVG format. Charts rendered using dc.js are data driven and reactive and therefore provide instant feedback to user interaction.
[d3.js](https://d3js.org/) | D3.js is a JavaScript library for manipulating documents based on data. D3 helps you bring data to life using HTML, SVG, and CSS. D3’s emphasis on web standards gives you the full capabilities of modern browsers without tying yourself to a proprietary framework, combining powerful visualization components and a data-driven approach to DOM manipulation.
[crossfilter.js](http://square.github.io/crossfilter/) | Crossfilter is a JavaScript library for exploring large multivariate datasets in the browser. 
[intro.js](https://introjs.com/) | Intro.js is an open source vanilla Javascript / CSS library to add step-by-step introduction or hints.
[Dashboard by Keen IO](https://keen.github.io/dashboards/)|  Responsive dashboard templates for Bootstrap.
[queue.js](https://d3js.org/) |  Lightweight asynchronous helper library used to load the character data from the database.
[Bootstrap](https://getbootstrap.com/) | Bootstrap is a framework that allows the user to easily create responsive websites based around a grid-like system.


### Project Detailed explanation

The graphs have an intro implemented through the use of 'introjs'. This detailed explanation will cover the 'behind the scenes' aspects of the project.
The usage of crossfilter/dc/d3 allows the dashboard to have an interactive chart system rather than a static one. The application then uses bootstrap to
create a visually appealing setup for the graphs.

The testing of the dashboard was performed manually. I used Chrome Developer tools to see the dashboard through the eyes of a mobile user and desktop user.
This allowed for me to ensure that all the aspects of the site are visible to mobile users. The testing was also performed on an iPhone 5 and a Huawei P9 lite.
The usage of Chrome and the mobile devices gave me enough insight in what problems the dashboard had and enabled me to fix any problems that I came across. I also
had some family/friends try the dashboard to have outside testing. The testers then informed me of mistakes with the dashboard through sending me screenshots or
writing down the problems they had. I then spent time replicating the problem and adjusting my code to fix the problem.


### Deploying Application

The application was deployed using "Heroku". Heroku is an easy to use deployment platform that easily integrates with github respositories.

The application was deployed in this manner:
1. The project was setup with Github to create a repository online.
2. Then Heroku can be linked up with github.
3. I set up Heroku with the option that Github changes were directly pushed to the app to allow for an instant preview of the updated application.
4. I used mLab, a free MongoDB add-on, to run the database for the application. The integration is easy and with the usage of Flask it's very efficient.
5. The dev version of the app includes a 'env' file that emulates a virtual machine. This is not needed with the Heroku application seeing as the "requirements" file handles the same function as the env.


### Testing
Function Tested | How it was tested
------------ | -------------
Start Tour button | The start tour button launches the introjs javascript. The feature was tested using the Chrome developer tools. The Chrome developer tools let me see the button on different device screens and ensure that it works regardless of the device. Once it worked perfectly on chrome, I tested the website on an iPhone and Android device to ensure that it worked on Desktop and mobile devices.
Reset Charts button | The reset Charts button was tested using Chrome Developer tools. I used the Chrome browser to test that it reset the charts and that it didn't create any errors in the process. I could see that through the console that's part of the Chrome Browser. Once it worked on Chrome, I again tested the feature on an iPhone and an Android device, to ensure that it worked on Desktop and Mobile.
Interactive Charts | The interactive Charts were tested using the Chrome browser. I used the console feature of the developer tools to catch any errors that the script would output and fix them as they happened. I then proceeded to have friends of mine visit the website from their Desktop or Mobile devices and try the website out. They then let me know what errors they found and I had them re-create the errors for me and then fixed the problem. This method of testing worked well, because it gave me outside insight of the dashboard and the appearance of it.
HTML Dashboard | The Dashboard uses Bootstrap to create the grid system. I used Chrome Developer tools to test the design of the site on different sizes of screens. Chrome allows you to test any size of device screen which helped me ensure that the dashboard is compatible with Desktop and mobile devices.



### External Influences

The general design of the dashboard was influenced by the dashboard example given during the course. The html skeleton 
was modified to fit my charts and the layout I required.

The font used in the chart headers is called [Parry Hotter](http://www.1001fonts.com/parry-hotter-font.html) and is free
to use for non-commercial projects.

