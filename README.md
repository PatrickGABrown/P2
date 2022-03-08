# Road Safety Analysis

## Project Description
In this project we were in a group of four and we were asked to find a big data set to perform analysis on. 
Our first task, of course, was to find data; we started by looking at the site for the Modeling the future challenge given that a part of this project was to come up with suggestions for decision making.  This site sent us data from the National Highway Traffic safety Administration.  This site provides a lot of diverse information related to vehicular accidents over a period of 25 years, so we then had to decide how we could narrow in some on this data for our project so it would have some coherency.
We decided to focus on the last four years given which was from 2016 - 2019. Given that traffic incidents tend, at least in our minds, to focus on motorized vehicles and their occupants, we decided we wanted to also emphasize something that the traffic administration also emphasized in their log—— how people outside vehicles, pedestrians and cyclists, are directly affected by these incidents. So, many of our more specific queries focus on those effects.
We utilized Apache Zeppelin to visualize the trends of our tables.

## Technologies Used
- IntelliJ/Emacs IDE with SBT(v 1.5.8)
- Scala (v 2.11.12)
- Spark lib dependencies (v 2.3.1)
- HDFS for storage of parquet files
- Git and GitHub for version control
- Magit (main git client for Emacs)
- Asana for project managmenet
- Apache Zeppelin for visualization

## Prompt
Create a Spark Application that process data(choose your data).

Size of data should be 2k and above,and a minimum 3 tables.

Your project  should involve useful analysis of data(Every concept of spark like rdd, dataframes, sql, dataset and optimization methods  and  persistence should be included). The Expected output is different trends that you have observed as part of data collectivley and how you can use these trends to make some useful decisions.

Should have admin and normal user access with password set in database along with Visualization  for out put 

Let the P2, have presentation with screen shots and practical demo.

## Trends
1. Age: (A)What are the trends across the age continuum effect the fatality rate of riders/drivers vs pedestrians? Essentially, what ages are most likely to die inside the car, and what ages are most likely to die outside of the car? Are they the same, do the trends have any similarities?
2. Big Picture: (B) Graph the trend of fatalities in entire USA, (C) then graph the trend of fatalities in individual states. What are the differences, do they all have the same basic movement upward and downwards? (D) Which states are safest (could be cross referenced with states with high public transport use to find correlation)?
3. Rural vs Urban: (E)(F)Combine rural state data together and urban state data together, compare graphed trends (specifically death rates of vehicle types, and overall death rates across time).
4. Vehicle: (G)(H)Find which vehicles are most dangerous to be around (kill passengers) vs most dangerous to be inside.

## Features
List of features ready and TODOs for future development:
- Utilized user/password settings to allow the user to create a user account and to enable setup of administrators to the app. The user can login and access a menu to choose queries that they would like to see on the data. The admin is able to set up other admin accounts and manipulate the tables in the app.
- Performed queries to discover trends of vehicle crash fatalities in the U.S. overall and in each individual state.
- Made analysis of the data received from the queries.
- Utilized SBT to package the project and run it from CLI.

To-do List:
- Use the SBT fat JAR file to run the app from AWS EC2s.
- Utilize machine learning to make predictive analysis on the data.
- Understand Apache Zeppelin on a deeper level.

## Getting Started
Use the git clone command in your terminal to clone this repo and be able to use it in an IDE:
```
git clone https://github.com/PatrickGABrown/P1.git
```
## Usage
- In your IntelliJ IDE, the main method is located in the P2.scala object in the src/main/scala path.
- You can also run the project by using sbt commands: sbt compile and sbt run.
- Once the project is running, the menu will appear for the user. The menu will prompt the user to login if they already have an account or create a new user account with a username and password.
- Once you login, there will be another menu for the user to choose which query they would like to see the results of.

## Contributors
Developed by Jessica(Optimization Lead), Jonathan (Visualization Lead), Justis (GitHub Admin/Owner, Team Lead), Patrick(Co-Admin/Lead).
