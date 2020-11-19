---
layout: post
title: Liberty, Equality, and Justice
subtitle: The fight to maintain Democratic Values established by our forefather
bigimg: /img/original.jpg
tags: [humanrights, classfication, peace]
---

We all believe in liberty, equality, and justice; those are the core values of democracy and America believes in it. The organization that I got to work with was Human Rights First, they are a non-profit organization who engages themselves for the betterment of society. They are in existence to challenge America to live up to its ideals, whenever the government and private companies fail to respect human rights and the rule of law they step in to demand justice, accountability, and reform.

I was so grateful to be part of the team that was assisting Human Rights First (HRF). I worked in finding data for police use of force, where human rights were being violated. Data can be so powerful to relay messages and show the world how our rights are being taken away from us. Our forefathers fought a great battle through experience and thought of many generations to draw up a constitution for the United States of America. If people in power fail to support the constitution, that’s when HRF steps in. After I was able to get some data related to police use of force, I had to make data relevant to the user story that we as a team was trying to solve. We wanted to solve a problem where users can easily view incidents where human rights were violated through an interactive map where they can select location, date, and types of use of force.

After finalizing the user stories, we as a team broke down user stories into shippable tasks. Since this was a cross-functional product, user stories were broken down into tasks that can be handled by data scientists, frontend, and backend. Here is the trello card for one of the user story.

![trello](/img/trello.jpg){: .center-block :}

For Data Scientists, we broke down tasks into parts where we had to scrape relevant data, explore data, do data engineering, finalize data to showcase the timeline of use of force, create endpoints to transfer data, build a Postgresql database on AWS RDS, and connect to it to have a highly stable database that safely stores data.

### Technical challenges and difficulties

![trello](/img/postgre.jpg){: style="float:left"}
This was an exciting project for me and for my teammates. To get to work with Human Rights First and help them on their journey of educating people of their rights and showcasing incidents that involved police use of force to show records to support how people have been mistreated and abused was a challenge, but that challenge brought the best out of everyone. I specifically worked on getting a route to communicate the timeline of police use of force within America.

For me personally, I was having technical difficulty connecting to the PostgreSQL in AWS RDS. I was wary of how I can connect to the database from                              various platforms like command prompt, and VS Code tool for PostgreSQL, which I tried but I was having trouble populating it with tables and data                                that I have acquired. Finally, after many trials and errors and searching on the internet for similar problems, I was able to use a management tool                              for PostgreSQL called pgAdmin.

### Teamwork makes the Dreamwork

The product is still under development. These four weeks of my life was very challenging, but I was able to accomplish a lot as well. As a Data Scientist for this project, I worked on getting relevant data, cleaning and feature engineering data, creating a route on FastAPI which was deployed on Elastic Beanstalk, creating a database on AWS RDS, and connecting it through pgAdmin to insert tables and data relevant to the project.

![trello](/img/get_timeline.gif){: .center-block :}

The future of this project looks bright. Although the upcoming team will be inheriting our work and developing on it, it will not be an easy task for them to finish the product. The challenges I foresee for the future are the path they want to take and how they want to describe the categories for police use of force, what user stories they would like to work on. They might not take the road we took and build something completely different like a predictive model that predicts types of police use of force.

I personally enjoyed working with my team, everyone was confident in their abilities and showed great respect and professionalism within the team. I also got to learn a lot from this experience working with great leaders and teammates. In the beginning, I was having a hard time understanding the project, and the role I will play within the team. I was able to carry through and continue with the project because of how my teammates understood me and pushed me to carry on through constructive feedback. I was lacking in confidence, communication, and patience, but I can say that I have improved a lot and this experience will help me to tackle future endeavors.

