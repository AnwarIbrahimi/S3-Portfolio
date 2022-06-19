# Portfolio Semester 3

## Table of contents

- Learning Outcomes
  - [Outcome 1: You design and build user-friendly, full stack web applications](#outcome-1-you-design-and-build-user-friendly-full-stack-web-applications)
  - [Outcome 2: Tooling and methodology](#outcome-2-you-use-software-tooling-and-methodology-that-continuously-monitors-and-improve-the-software-quality-during-software-development)
  - [Outcome 3: Agile](#outcome-3-you-choose-and-implement-the-most-suitable-agile-software-development-method-for-your-software-project)
  - [Outcome 4: Design and implement ](#outcome-4-you-design-and-implement-a-semiautomated-software-release-process-that-matches-the-needs-of-the-project-context)
  - [Outcome 5: Cultural Differences](#outcome-5-you-recognize-and-take-into-account-cultural-differences-between-project-stakeholders-and-ethical-aspects-in-software-development)
  - [Outcome 6: Requirements](#outcome-6-you-analyze-non-functional-requirements-elaborate-architectural-designs-and-validate-them-using-multiple-types-of-test-techniques)
  - [Outcome 7: Business Process](#outcome-7-you-analyze-and-describe-simple-business-processes-that-are-related-to-your-project)
  - [Outcome 8: Professional manner](#outcome-8-you-act-in-a-professional-manner-during-software-development-and-learning)
  
## Learning Outcomes 

### Outcome 1: You design and build user-friendly, full stack web applications
You apply basic User experience testing and development techniques.

#### What does this learning outcome mean?
You design and build a full stack application using commonly accepted front end (Javascript-based framework) and back end techniques (e.g.,
Object Relational Mapping) choosing and implementing relevant communication protocols and addressing asynchronous communication issues.

#### What will i do for this learning outcome?
For this Learning Outcome i will create a full stack web application which consists of a backend and frontend. For the frontend i will be using React as the framework. I'm also using the movie database API to get up to date movies and series. For the backend i'm using Springboot and i will also make my own REST API. 

#### What have i done for this learning outcome?
For this learning outcome i started with doing research in the frameworks and best practices. You can find the research down below with links to the research document. After i was done with the research i started by watching a **Tutorial: https://www.youtube.com/watch?v=XkVpb_8IPUM&t=5488s** and followed this example to start my own backed project with springboot. after some testing and following the examples i had a base idea of how things worked in the backend. After this i switched to the frontend which i used **React** for. Since i'm using an API to get the movies and series for my application i started out with this. I used **AXIOS** to make API calls. example of these calls where documented by the Online API i found **themoviedb** https://developers.themoviedb.org/3/getting-started/introduction. After i made the connection with the API i started working on the frontend. I started with the homepage and from there out i had a foundation for my application. from there out i expanded the application bit by bit.

For the frontend i chose Javascript and for the framework react. More on why i chose this you can find in my research with the link below.
- [Frontend Development](https://github.com/AnwarIbrahimi/S3-Portfolio/blob/main/Research.md#frontend-development)

For the backend i went with java as this was a new language for me and i wanted to learn something new. And for the framework i went with springboot. More on this and why i chose this you can find in the link below.
- [Backend Devlopment](https://github.com/AnwarIbrahimi/S3-Portfolio/blob/main/Research.md#backend-devolepment)

![image](https://user-images.githubusercontent.com/99720686/164415594-d53aa84f-4dc7-45cf-8d78-60fb8b0296fd.png)

![image](https://user-images.githubusercontent.com/99720686/164415664-b38217da-d226-410f-bbf1-56a3d2677590.png)


### Outcome 2: You use software tooling and methodology that continuously monitors and improve the software quality during software development.
#### What does this learning outcome mean?
Carry out, monitor and report on unit integration, regression and system tests, with attention for security and performance aspects, as
well as applying static code analysis and code reviews.

#### What will i do for this learning outcome?
For this Learning Outcome i will assure software quality and tools to make that work. In order to make that work i will need to make different kinds of tests. Which exact tests this will be i need to look more into. This will be functional and non-functional tests. Part of this will also be automation tests. To assure this i will implement a CI/CD pipeline with github actions. I also need to look at what test i will use for the different parts in my project.

#### What have i done for this learning outcome?

#### What is testing?
Software Testing is a method to check whether the actual software product matches expected requirements and to ensure that software product is Defect free. It involves execution of software/system components using manual or automated tools to evaluate one or more properties of interest. The purpose of software testing is to identify errors, gaps or missing requirements in contrast to actual requirements.

#### Why is testing important?
Software Testing is Important because if there are any bugs or errors in the software, it can be identified early and can be solved before delivery of the software product. Properly tested software product ensures reliability, security and high performance which further results in time saving, cost effectiveness and customer satisfaction.

#### What different kinds of tests are availiable?
It's important to make the distinction between manual and automated tests. Manual testing is done in person, by clicking through the application or interacting with the software and APIs with the appropriate tooling. This is very expensive since it requires someone to setup an environment and execute the tests themselves, and it can be prone to human error as the tester might make typos or omit steps in the test script.

Automated tests, on the other hand, are performed by a machine that executes a test script that was written in advance. 

#### Unit tests
Unit tests are very low level and close to the source of an application. They consist in testing individual methods and functions of the classes, components, or modules used by your software. Unit tests are generally quite cheap to automate and can run very quickly by a continuous integration server.

#### Integration tests
Integration tests verify that different modules or services used by your application work well together. For example, it can be testing the interaction with the database or making sure that microservices work together as expected. These types of tests are more expensive to run as they require multiple parts of the application to be up and running.

#### End-to-end tests
End-to-end testing replicates a user behavior with the software in a complete application environment. It verifies that various user flows work as expected and can be as simple as loading a web page or logging in or much more complex scenarios verifying email notifications, online payments, etc...

End-to-end tests are very useful, but they're expensive to perform and can be hard to maintain when they're automated. It is recommended to have a few key end-to-end tests and rely more on lower level types of testing (unit and integration tests) to be able to quickly identify breaking changes.

#### Which tests will i be using and why?
I will make use of **unit tests** to ensure that the functions of my classes work correctly. The unit tests that i will be making will mostly be for
the crud operations i made. Besides unit tests i will also make **end-to-end tests** to make sure that the user flow works as expected. And last but not least i will make **integration tests** to make the different components of my application works wel together. 

#### SonarQube
To use static analyse code i used sonarqube. I implemented sonarqube with **Gitlab CI**. Below you will find the screenshots of the analysed code. and the yaml file i used in my repository. i will also explain what i learned about the analysed code and what i can do to improve my code.

![image](https://user-images.githubusercontent.com/99720686/174304160-0403e3c6-0007-40b4-8f7c-6b88814d59fa.png)

As you can see i have 3 vulnerabilities to fix this i can implement a DTO to get rid of the vulnerabilities in my project.

![image](https://user-images.githubusercontent.com/99720686/174304643-c8595693-8ee2-4ec0-a833-98bddd363d97.png)

### Performace testing
To test the performace of my appication i used google lighthouse. As a result which you also see in the screenshot below i scored 61 on performance which isn't the greatest. the main reason it isn't higher is bascially because how my application works. I get a lot of data from movies and series which lowers the performance of the application. there is also a lot of pictues the website needs to load. Considering all this the score could be worse. A fix for this would be too minimize the amout of pictures the website has to load on one page and make them smaller. This should bump up the performance by quite a bit.

![image](https://user-images.githubusercontent.com/99720686/174306893-c9ddd2a6-edf6-47e1-a62d-af715e1fad6b.png)

### Outcome 3: You choose and implement the most suitable agile software development method for your software project
#### What does this learning outcome mean?
You are aware of the most popular agile methods and their underlying agile principles. Your choice of a method is motivated and based on
well-defined selection criteria and context analyses.

Agile is a way or approach to project manegement for developers that helps projects and the people that are working on it. An agile team works in smaller sprints usually around 3 or 4 weeks. a sprint consist out of a sprint backlog, daily standups, sprint review and a retrospective.
![agile](https://user-images.githubusercontent.com/99720686/169487945-b38a0a34-8bd1-4ca0-b48c-5133b7043daa.jpg)

There also is a **agile manifesto** which outlines 4 values and 12 principles one example of this is: **Individuals and interactions** over processes and tools. There also is the scrum model. This is a way of working with fixed iterations that give agile teams a framework for producing software with regular feedback and feedback is one of the most important thingw if it comes to working with agile.

#### What will i do for this learning outcome?
For thid learning outcome i will work with agile principles and methods and improve myself during the semester. In order to achieve this me and the group use some of the popular agile methods like product backlog, sprint backlogs, sprint reviews, retrospectives and daily standups. besides that i will do research in agile and make a report of my findings.

#### What have i done for this learning outcome?
To use agile methods and principles in the group we use github. In github we make use of a **sprint backlog**. We made user stories as issues. We are also making use of a **product backlog**. This is defined in a board. This board is being updated at the start of every sprint. Below you can find the links of the backlogs. At the end of sprint we do a sprint review. To do this we make a powerpoint with the the tasks we planned to do at the start of the sprint and what we succeeded at the end of the sprint. We also reflect on the sprint. All this we do in front of the client and we get feedback from them. This feedback is documented and we also take this into the retrospective. As scrummaster in a retropsective i make sure that everyone understands what the meeting means and that the meeting doesn't take too long.

- [Product Backlog](https://github.com/AnwarIbrahimi/Netmatch/issues)
- [Sprint Backlog](https://github.com/AnwarIbrahimi/Netmatch/projects/3)

An extra step we do with user stories besides that we have a overview with all the user stories we go into depth with what a user story exactly is 
and what the steps are to complete one. In order to do this we write on a whiteboard step by step what a user story really consists out of different layers. 

As i explained above agile is an approach to project management and software devolopment. Agile also has a Mainfestio whitch outlines 4 values and 12 principles for teams and are as followed. 

**Individuals and interactions** over processes and tools

**Working software** over comprehensive documentation

**Customer collaboration** over contract negotiation

**Responding to change** over following a plan

### **The 12 principles behind Agile Manifestio:**

Our highest priority is to satisfy the customer
through early and continuous delivery
of valuable software.

Welcome changing requirements, even late in
development. Agile processes harness change for
the customer's competitive advantage.

Deliver working software frequently, from a
couple of weeks to a couple of months, with a
preference to the shorter timescale.

Business people and developers must work
together daily throughout the project.

Build projects around motivated individuals.
Give them the environment and support they need,
and trust them to get the job done.

The most efficient and effective method of
conveying information to and within a development
team is face-to-face conversation.

Working software is the primary measure of progress.

Agile processes promote sustainable development.
The sponsors, developers, and users should be able
to maintain a constant pace indefinitely.

Continuous attention to technical excellence
and good design enhances agility.

Simplicity--the art of maximizing the amount
of work not done--is essential.

The best architectures, requirements, and designs
emerge from self-organizing teams.

At regular intervals, the team reflects on how
to become more effective, then tunes and adjusts
its behavior accordingly.

### **Extreme Programming (XP)**
In the group project we were mainly using the scrum method. In addition to the scrum method there are different agile methods to use. One of these is the Extrexe Programming (XP) one. XP is a method that emphazizes teamwork, communicatioin and feedback. It focuses on constant development and feedback from the customer. Almost the same as scrum. XP also uses short sprint and development cycles so in a way we were also doing XP while doing scrum. XP is mostly being used in a situation where the requirements of a custsomer varies alot. It also allows the developers to keep up with these demands.

### **Conclusion**
Working with the agile methodology has been very useful this past few months. Myself and the group have come a long way adapting to the method and evolved as a group and individuals. Choosing a agile method also depends on the project and the situation. The best thing to do is to look at the advantages and disadvantages of a method and choose one after that.

### Outcome 4: You design and implement a (semi)automated software release process that matches the needs of the project context.
#### What does this learning outcome mean?
You design a release process and implement a continuous integration and deployment solution (using e.g. Gitlab CI and Docker).

#### What will i do for this learning outcome?
For this Learning Outcome i will implement CI/CD with github actions. I will also will be using Docker Desktop for the Docker container. 

#### What have i done for this learning outcome?
For tis learning outcome i started out by doing some research in CI/CD and what CI/CD exactly does. I started out by reading through the **Canvas Module**. from there out i looked for best practices. Since i was already used Github for my project the best practice for me would be to use github actions to implement CI/CD. Now that i made my choice on what to use i started out by following a tutorial and implemented CI/CD. i used **Docker Desktop** to build the container. There were some problems along the way during the implementation. one problem whas that it just didn't wannted to build when deploying it. after some searching on google i found a solution on stackoverflow with some code that i needed to add in my pom file and this fixed the issue.

#### CI/CD
CI/CD is a method to deploy automation into developing. CI/CD stands for continous integration, continious delivery and continious deployement

To implement CI/CD i used github. Below you can see the worflow i used. 
![image](https://user-images.githubusercontent.com/99720686/164418209-65d96173-1875-4535-8169-82a084c2c73f.png)

Below you can see the docker push image i used. I'm also using docker desktop to push out the containers.
![image](https://user-images.githubusercontent.com/99720686/164418863-73553fc9-2aef-4ef6-9406-5037f3631136.png)

![image](https://user-images.githubusercontent.com/99720686/164448231-74bb6fa8-b094-40a2-94e0-2b4ad18d2db1.png)


### Outcome 5: You recognize and take into account cultural differences between project stakeholders and ethical aspects in software development.
#### What does this learning outcome mean?
Recognition is based on theoretically substantiated awareness of cultural differences and ethical aspects in software engineering.
Adapt your communication, working, and behavior styles to reflect project stakeholders from different cultures;
Address one of the standard Programming Ethical Guidelines (e.g., ACM Code of Ethics and Professional Conduct) in your work.

#### What will i do for this learning outcome?
For this Learing Outcome i will explain the diffrences in the different cultures and how this affects us as a group. I am also gonna make a personality test.

#### What have i done for this learning outcome?
I have made a personality test for the LO Cultural Differences. The result i got is that i am a leader. I can see myself being this since i was the group leader in previous semensters and i am the scrummaster this semester. As a leader i take initiative in the group. 

### Culture
#### **What is culture?**
>  “For the purposes of the Intercultural Studies Project, culture is defined as the shared patterns of behaviors and interactions, cognitive constructs, and affective understanding that are learned through a process of socialization. <br> 
These shared patterns identify the members of a culture group while also distinguishing those of another group.“ 

For me culture is defined by where you come from and where you grow up as a person. This also effects the choices you make in life. 

#### **Which are well-known dimensions on cultural differences?**
> “Geert Hofstede, in his pioneer study looking at differences in culture across modern nations, identified four dimensions of cultural values: individualism-collectivism, power distance, uncertainty avoidance, and masculinity-femininity. Working with researcher Michael Bond, Hofstede later added a fifth dimension with called dynamic Confucianism, or long-term orientation. According to Hofstede’s research, people, in individualistic societies, are expected to care for themselves and their immediate families only; while in collectivist cultures, people view themselves as members of larger groups, including extended family members, and are expected to take responsibility in caring for each other. With regards to power distance, different countries have varying levels of accepting the distribution of unequal power.“

From what i have read from the different dimensions on cultural differences. these sounds fimiliar to me especailly in the high power distance countries.

#### **Can you give examples for cultural differences that you have experienced in your study or life? How do you explain these differences?**
A example that i have encounterd in my life and the difference in my culture and other cultures is the way people greet eachother. In one culture it's very normal to give kisses to eachother and in other cultures people give a hand.

#### **What is your culture?**
My culture is north-african, but i'm born and grew up in the Netherlands. So am i mix of both i would see. A part of me follows the african cultures and the other part the dutch culture.

### Ethics
#### **What is ethics in software engineeering?**
Software engineering ethics can be approached from three directions. First, it can
describe the activity of software engineers making practical choices that affect other
people in significant ways. Second, it can be used to describe a collection of principles,
guidelines, or ethical imperatives that guide or legislative action, and third, it can be used
to name a discipline that studies the relationship between the other two senses of ethics.
Software engineering ethics is clearly both an activity and a body of principles. The
discipline of software engineering ethics that studies this activity and formalizes these
principles, however, is in its infancy.

#### **Why is ethics important in software engineeering?**
Ethics in software engineering leads employees and employers to understand the importance of practicing ethics in software engineering with the digitalizing workplace. So, when an ethical problem arise it has to be resolved straightforward under any circumstance or else unmanaged ethical problems will definitely will cause a serious problem.

#### **Which ethical aspects play a role in your project?** 
Ethics in my project would be professionaly communicating with eachother but also towards teachers and stakeholders. This also plays a role in asking feedback. When aksing feedback i try to come prepared and pepare the right things so we can have a professional conversation.

![image](https://user-images.githubusercontent.com/99720686/164412887-3ae43775-7a1b-4fe8-85c7-edad1869dd0e.png)

### Outcome 6: You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using multiple types of test techniques
#### What does this learning outcome mean?
You apply user acceptance testing and stakeholder feedback to validate the quality of the requirements. You evaluate the quality of the design
(e.g., by testing or prototyping) taking into account the formulated quality properties like security and performance.

#### What will i do for this learning outcome?
For this learning outcome i will be making a C4 Model. This will be part of my architecture document. In addition i have a Analyse document with different
user stories and requirements of my application.

#### What have i done for this learning outcome?
For this learning outcome i made a C4 model to have a view of the architecture of my application. I also made requirements and out of these requirements i made user stories examples of these are below.

- [Architecture](https://github.com/AnwarIbrahimi/S3-Portfolio/blob/main/Architecture.md)
- [Analyse](https://github.com/AnwarIbrahimi/S3-Portfolio/blob/main/Analyse.md)

#### How did we validate the requirements and design with the stakeholder?
At first we had a meeting with the stakeholder and asked questions about what they wanted to see in thier application and what thier requirements were. After the meeting we discussed what the best way is to implement these requirements and made some wireframes and requirements. In the next meeting we went over the requirements and wireframes and we set piorities in what order which requirements had priority.

![image](https://user-images.githubusercontent.com/99720686/174300058-7be6691e-2106-452a-89e9-4ee5ee38bb10.png)

### Outcome 7: You analyze and describe simple business processes that are related to your project.
#### What does this learning outcome mean?
Involving stakeholders, predominantly sequential processes with one or two alternative paths. Business processes during which the software that you are developing
will be used (business processes that the software must support by fully or partially automating them). or Business processes needed for the success of your software
development project (e.g., product release, market release, financial assurance).

#### What will i do for this learning outcome?
For this Learning outcome i will do research into the business process and how this affects my project. 

#### What have i done for this learning outcome?
#### **What is a business process?**
Business process management (BPM) is a systematic approach to improving those processes, which helps organizations achieve their business goals. If an organization is unable to perform certain business processes internally due to cost or resource constraints, the company might use business process outsourcing. Many organizations contract specific business tasks -- such as payroll, human resources (HR) or accounting -- to a third-party service provider.

#### **How a business proces relates to software applications?**
A structured business process carries out a pre-defined sequence of steps. The process might have many options, with different steps carried out by different instances of the process at different times. Still, the creators of the process determined what the possible steps were in advance. When a structured business process is supported by an application, it’s common for the software to implement the complete process. Think of an automated manufacturing process, for example, where an application directs a group of machines to repeat the same steps over and over. In situations like this, people primarily provide inputs, accept outputs, and handle exceptions. The software carries out the process itself.

#### **Does my software automate a task, facilitate a task, or make a new task possible to perform?** 
The software i'm making does not automate a task. however during my internship we automated a process and thats what i am going to talk about. The process we automated was when someone came to the helpdesk they needed to wait for someone to come over to help them. To automate this process we created software which could be used on the tablet at the desk. With the software you could fill in what you needed and it told you what to do. Through this process the customer didn't have to wait for a worker to come over them and the worker didn't have to come over. 

#### Business process diagram
![image](https://user-images.githubusercontent.com/99720686/174477984-4554eb44-cc3d-4365-b001-54ffa7202cbc.png)

### Outcome 8: You act in a professional manner during software development and learning
#### What does this learning outcome mean?
You actively ask and apply feedback from stakeholders and advise them on the most optimal technical and design (architectural) solutions.
You choose and substantiate solutions for a given problem.

#### What will i do for this learning outcome?
For this Learning outcome i will continiously ask feedback and work with this feedback. Besides that i will also make a STARR reflection. 

#### What have i done for this learning outcome 
For this learning outcome i made a STARR reflection on the sitation and communiction i have with the stakeholders and teachers this also includes feedback

![STARR](https://user-images.githubusercontent.com/99720686/169486147-c5d82dd3-d95e-4aee-b688-c3f625a97af7.png)

**Situation**: During the end of the sprint we had a sprint review with the customer and i took leed on the presentation.

**Task**: My task was in the presentation was to talk about the past 3 weeks about what we did as a group and what succedeed and what went wrong. 

**Action**: During the presentation i went through the requirements we had discussed. I lined them up and when through each of them. I validated with the stakeholder if these are still the requirements they wanted and if we implemented them the way they want.

**Results**: As a result we had a good overview of which requirements were the priority and in which way these requirements should be made.

**Reflection**: The presentation went smoothly for the most part. We could ask the quesions we wanted and the stakeholder was happy. What i could do better for the next presenatation is to let other peoplpe talk too. This was also feedback from the stakeholder to try and let everyone have a say in the conversation. To do this i will make an agenda to give everyone a tasks to make sure everyone has something to say at the presentation.

