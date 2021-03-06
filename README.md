# What To Watch (WTW)

Wondering What To Watch? [Try this here!](https://what-to-watch-project.herokuapp.com/)

What To Watch project is a website for sharing and finding media suggestions to other 
users like movies, series, documentaries etc.
It's an easy and quick way to answer the often asked question when we are sitting on the 
couch with the remote in our hands for example and thinking  - What to watch? 

![responsive design image](static/images/responsive/responsive_ms3.PNG)

## User Experience (UX)

### User Stories

* As a visitor, I want to understand quick and easy what the website is about.
* As a visitor, I want to be able to get ideas for my search directly from the openning page of the site. 
* As a visitor, I want to easily navigate and find all content easy to read and all options easy to use.
* As a user, I want to be able to share or add content on the website as my personal suggestion.
* As a user, I want to be able to see list of movies from specific genres.  
* As a user, I want to be able to find further information about a contant that I'm interested in watching
 via additional links for example. 

### Design

#### Color Scheme

In WTW website the main combination of colors are:

1. #424242 - dark grey for header, footer, buttons and most of the content holding elements. 
2. #80cbc4 - light cyan color for buttons and forms 
3. Black and White for text depending on the backgraoud.   

#### Typography

The Google Fonts Cabin font is used throughout the whole website with Sans Serif as the fallback font in case the font
isn't being imported into the site correctly.

### Wireframes

* Mobile Device
   * [Home Page](https://raw.githubusercontent.com/dimitar-4/ms3-what-to-watch/master/static/images/wireframes/home%20mobile.png)
   * [All Movies Page](https://raw.githubusercontent.com/dimitar-4/ms3-what-to-watch/master/static/images/wireframes/movies%20mobile.png)
   * [Add Movie Page](https://raw.githubusercontent.com/dimitar-4/ms3-what-to-watch/master/static/images/wireframes/add%20mobile.png)

* Desktop Device
   * [Home Page](https://raw.githubusercontent.com/dimitar-4/ms3-what-to-watch/master/static/images/wireframes/home%20pc.png)
   * [All Movies Page](https://raw.githubusercontent.com/dimitar-4/ms3-what-to-watch/master/static/images/wireframes/movies%20pc.png)
   * [Add Movie Page](https://raw.githubusercontent.com/dimitar-4/ms3-what-to-watch/master/static/images/wireframes/add%20pc%20.png)

## Features

### Existing

What To Watch website is responsive on mobile and desktop devices. Delivers a good contrasting color scheme for 
the content, navigation menu, footer and all buttons throughout the website for better user experience.

The website WTW is also containing CRUD(Create, Read, Update, Delete) functionality so the user can:
   * Create new content on the website from the 'Add Movie' link in the navbar.
   * Read the content on the website fro the 'All Movies' link in the navbar where is a complete list of the database content.
   * Update an item's information by clicking on it and then select the 'Edit' button.
   * Delete an item from the database by clicking on it and then select the 'Delete' button.

The User can also filtering movies database by different genres.

### Left to Implement 

   * Adding a register user, Log In/Out options so that the user can still see all the content in the website but restrict the access 
to the edit and delete functionality to the items that were created only by specific user.
   * Adding a comments sections where different users can share their opinions about the website, or specific item on the website. 


## Technologies Used

### Languages Used 

* HTML5
* CSS3 
* Python
* JavaScript

### Frameworks, Libraries & Programs Used

1. Google Fonts
   * Used Cabin font for the website. 
2. Font Awesome
   * Used to add icons for better visual appealing. 
3. jQuery
   * Used for responsive and interactive design for the website.
4. Materialize
   * Used librery for responsiveness and adding style. 
5. Balsamiq
   * Used to create wireframes for the basic look of the website.
6. MongoDB
   * Used to create and store database for the website.
7. Heroku
   * Heroku is the platform where the website is being deployed.
8. Git
   * Used for version control by Gitpod's terminal commit to Git and push to GitHub.
9. GitHub
   * GitHub is where the project's repo is stored after being pushed from Git.

## Testing

### UX Testing

 What To Watch(WTW) website provides users with easy and simple to use layout. Easy to understand 
 content and navigate throughout the app with a short menu on the top right.

 With the home page users receive short and clear description about the purpose of the website.
Directly under the description can be found top rated suggestions that can already give an idea 
to the user What To Watch.
Under that the user can get familiar with what the rating numburs mean if the goal is to interact 
with the app to add content. 
After that there is a easy and quick way to filter all movies based on their genre, so the user can
get a list of suggestions only from the genre he like.

At the bottom in the footer element links are provided that can further inform the user for a movie 
he finds interesting to check out.

In The 'All Movies' page the user can view all containing movies and also filter by genre. By clicing on a movie 
the coplete info about it is showing in a pop out window where also can interact further with the data with the 
Edit and Delete buttons. 

In the 'Add Movie' page users can add content they like and want to recommend to other users.

All functions WTW app provides were tested on different devices and by the developer, frends and family and no 
issues were shown during testing.

### Browsers and OS Testing
   
   WTW was tested on:
   * Chrome
   * Edge
   * Android
   * iOS 

   No issues were found during testing.

### Device Testing

WTW is tested on:
   * Samsung Galaxy S20 FE
   * IPhone 10 Pro
   * Huawei P20 Pro

Other devices tested:
   * Acer Aspire 5 A515-51G
   * Acer B7 series-B277(Desktop Monitor)

### Links Testing

All links and buttons are tested. No problems were shown on tested devices.

### Problems

Search bar is not included in the project like it is shown in the wireframes beacause 
there was issues creating a text search index and until the project deadline solution was not found.
It will be added in the future, but for now after communicating with mentor, tutor support and other 
students on Slack I couldn't fix the problem. I tried like in the CI 'Putting it all together' mini-project 
videos, I tried directly in MongoDB and in my app.py file but either no result in MongoDB or getting errors.   

## Deployment

1. Createing GitHub repository for the project website.
2. Creating all necessary files in the GitPod workspace that Heroku needs to deploy the project 
and pushed them to GitHub.
3. Open Heroku.com and logged in, then in the upper right corner clicked on New/Create New App.
   * Selected unique name for the app and chose region.
4. When the app were loaded from the menu under the app title chose Deploy.
5. From the available deployment methods chose GitHub(Connecting to GitHub)
6. After clicking on GitHub under the deployment methods checked if the right GitHub profile is displayed, 
and added the repository name for the project and clicked on the search button.
7. When the repository was found and displayed clicked on the connect button under to connect the GitHub repository 
with Heroku.
8. Then, up to the menu again and clicked on settings.
9. In settings clicked on 'Reveal Config Vars'.
   * There added key-value pairs for the required variables since a hidden python file contained environment variables.
10. Clicked on the deploy option again from menu above and enabled the automatic deployment.  
11. Selected wich branch(master) of the GitHub repository to be deployed and clicked 'Deploy Branch'.
12. After the build was done a "Your app was successfully deployed" message was displayed with a 
button 'View' to open the website.
13. Link to the project's GitHub repository [here!](https://github.com/dimitar-4/ms3-what-to-watch)
14. Live link from Heroku [here!](https://what-to-watch-project.herokuapp.com/) 

## Credits

### Code 
   * The code for WTW project is following most of the steps shown in the Code Institute's 'Putting it all together' 
   mini-project for building a task menager. What To Watch project's foundations are based on the code from 
   those lesson series.
   * Throughout the development process solutions for some code related problems were found in [StackOverflow](https://stackoverflow.com/) 

### Content
   * All information about movie database is from [IMDb](https://www.imdb.com/) website.
   * All other text is written from the developer.

### Media

   * The background image for the website is from [Pinterest](https://in.pinterest.com/)

### Acknowledgements
   * Akshat Garg (mentor) - THANK YOU for the advices, guidance, feedback and patience throughout the developing process of WTW project.
   * Inspiration about the What To Watch project came from the same question I often ask my self or being asked from other people. The need 
   for place where recommendations, good ideas can be stored and answer that question easy and fast.
   * Slack - a lot of good and helping people there - thank you!