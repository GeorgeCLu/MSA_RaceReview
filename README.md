# RaceReview

https://racereviewmsa.azurewebsites.net/ is a sample site designed for users to submit reviews and ratings of past motor races such as Formula 1.
Please note that the database may need to spool up, so please refresh if there is no data displayed.
It is aimed to answer the commonly asked question of which past races to watch, so that other users can find races and their reviews and decide to watch or not.

![Alt text](reademeImages/2.png)<br/><br/>
![Alt text](reademeImages/5.png)<br/><br/>
![Alt text](reademeImages/6.png)<br/><br/>
![Alt text](reademeImages/7.png)<br/><br/>
![Alt text](reademeImages/9.png)<br/><br/>
![Alt text](reademeImages/10.png)<br/><br/>
![Alt text](reademeImages/12.png)<br/><br/>
![Alt text](reademeImages/13.png)<br/><br/>
![Alt text](reademeImages/14.png)<br/><br/>

The frontend Typescript React web app connects to a REST API which is a ASP.NET Core Web Application, both of which are hosted as Azure web apps.

The server uses the Entity Framework to connect to an instance of Azure SQL database in a serverless configuration.

Backend code is at https://github.com/GeorgeCLu/MSA_Race_ReviewAPI

SignalR chat code is at https://github.com/GeorgeCLu/racereviewchat_signalR

Links to folder containing completed Microsoft Learn modules and demo video:
https://drive.google.com/drive/folders/1BDGsVCO6WIxaiVE4gxv2SqvSlKcXgUup?usp=drive_link

Individual link to demo video (Apologies audio may not be great, please see the readme for a further explanation of the features:
https://drive.google.com/file/d/15-_9evaxLcczfSfHqCN0-sSmJ4WpzYNU/view?usp=drive_link

Current functionality listed below.

Basic features:
<ul>
  <li>React Project using Typescript</li>
  <li>Uses Material UI</li>
  <li>Responsive on both desktop and mobile</li>
  <li>React Route</li>
  <li>Git usage (both front and backend)</li>
  <li>Built using C# using .NET CORE 6</li>
  <li>Uses EFCore</li>
  <li>Persists data using to a SQL database in Azure</li>
  <li>CRUD operations</li>
</ul> 

Advanced features:
<ul>
  <li>Usage of web sockets (Uses SignalR, which is built on top of web sockets</li>
  <li>Use of AI technologies in your project (Uses voice recognition to transcribe speech to txt, so it can be posted for a review</li>
  <li>Deployed using Azure (Using Azure web apps)</li>
</ul> 

Most proud of the real-time chat functionality, built using SignalR, as well as as the voice recogition for the reviews

There is a desktop view and a mobile view where the tackbar collapses to a drawer.
![Alt text](reademeImages/32.png)<br/><br/>
![Alt text](reademeImages/36.png)<br/><br/>

The theme of the site is inspired by chicanes in racing circuits.

Without logging in, users can see the list of races and see its details and also its average score and total number of reviews. 
![Alt text](reademeImages/15.png)<br/><br/>

Clicking on a race's page will show user reviews and their scores for that race, which can be upvoted or downvoted.
![Alt text](reademeImages/29.png)<br/><br/>

Users can search for races such as the race name and location or sort them by criteria such as the average score.
![Alt text](reademeImages/20.png)<br/><br/>

Currently to login there is no backend authentication for logging in, so any username and password is accepted.

Once logged in, the user can add races to the database.

![Alt text](reademeImages/30.png)<br/><br/>

Logged in users can submit or edit or delete their reviews and scores for the races.
![Alt text](reademeImages/28.png)<br/><br/>

Once a review is submitted, the average score and total number of reviews will update.
![Alt text](reademeImages/25.png)<br/><br/>

Logging in as 'Admin' with 'password' as the password, gives full admin privileges, and can edit/delete races or other user's reviews.

In Chrome only, for the review it uses the Web Speech API, so the user's voice input can be converted to text in the review box.
It will listen for several spoken sentences.

![Alt text](reademeImages/31.png)<br/><br/>

In the chat tab, logged in users can live chat to each other.
The chat service is run as a Azure Function app which then connects to an instance of Azure SignalR service.
![Alt text](reademeImages/34.png)<br/><br/>
![Alt text](reademeImages/35.png)<br/><br/>

Backend code is at https://github.com/GeorgeCLu/MSA_Race_ReviewAPI

SignalR chat code is at https://github.com/GeorgeCLu/racereviewchat_signalR
