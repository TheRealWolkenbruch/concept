# AreYouThere?

> Asking the simplest questions sometimes helps, especially during corona-times: **Are you there?**

## Preamble

This project was handed in as a contribution to the [EU vs. Virus Hackathon](https://euvsvirus.org/) in April 2020.

- On Github: https://github.com/TheRealWolkenbruch/
- On DevPost: https://devpost.com/software/areyouthere
- Participants (in alphabetical order):
  - [doggygit](https://github.com/doggygit) - Backend Development & Databases
  - [Garllon](https://github.com/Garllon) - Backend Development & Databases
  - [hendrikb](https://github.com/hendrikb) - Project Lead & Backend Development & Operations
  - [omarsotillo](https://github.com/omarsotillo) - Frontend Wizard & Design
  - [randres1640](https://github.com/randres1640) - Backend Development & Databases
  - [Thudilie](https://github.com/Thudilie) - Frontend Wizard & React Developer

First of all - a big, big Thank You to all of you! :rocket:

## The problem your project solves

Staying in contact became significantly harder in early 2020.

Before corona, it was easy to just hop on to a train and check whether your good friend is doing fine or your grandmother needed something. Now you want to avoid public transportation or it's impossible to see someone, because they are quarantined.

## The solution you bring to the table (including technical details, architecture, tools used)

### Approach

We built a web-based service that allows __Guardians__ to look after people, who need to be looked after every now and then - we call those people __Wards__. :)

AreYouThere is a low-threshold service that can be used to collect "I'm doing good"-feedback as well as additional information about the Wards - such as "current mood" or requests for assistance - if the respective person wants to provide further input.

The service sends out regular reminders to the Wards - if there's no response from a Ward within a specified time range - the respective Guardian receives an alert and can act.

### Technology

We provide source codes for the two main components of the service:

- The **Backend API** ...
  - ... source code is available here: https://github.com/TheRealWolkenbruch/are-you-there-api
  - ... is a [ruby](https://www.ruby-lang.org/en/)-based microservice API implemented mainly in [roda](https://github.com/jeremyevans/roda)
  - ... provides _all_ methods and entities/components that our service requires, including [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) for our entities and Auth-related things
  - ... can be deployed using docker since it's available on dockerhub: https://hub.docker.com/r/areyouthere/api

- The **Frontend App**:
  - ... source code is available here: https://github.com/TheRealWolkenbruch/are-you-there-ui
  - ... is a stateless [React](https://reactjs.org/)-based static frontend application that speaks to the Backend API
  - ... provides _all_ graphical user interfaces for our service 
  - ... can be deployed using docker since it's available on dockerhub: https://hub.docker.com/r/areyouthere/ui

### Deployment

We are encouraging individuals to run a copy of our software on their own behalf, that is one of the main reasons why we provide all our source codes.

We'll set up a proof-of-concept website soon, but in order to have your data and the data of your loved-ones under your control, you should strongly consider setting up this service for yourself.

The deployment is done through [kubernetes](https://kubernetes.io/) - the codes for that will be provided at a later point in time.

### Development

We rely heavily on [GitHub](https://github.com)-based workflows. Feel free to fork our project or contribute by posting issues or pull request.

Give us a :star: - we consider at a donation & thank you.

### The Result + What is missing

We achieved to have the basic function of the service working. It is a prototype that has been put together in only a few hours to demonstrate the purpose.

Please pay attention to the fact, that the application is **not even closely ready for production**. Major features are missing, layouts have to be optimized and security as well as professional quality assurance certainly fell victim to the hackathon's time constraints. We are aware of that and will continue working on those aspects.

### Business Goals & Monitization

We do not plan to monetize this project.

Our main goals were to provide a meaningful contribution to the society in corona times, to learn some new technologies and experience a major hackathon. We achieved our primary goals.

However, we plan to continue on this project and set up a working instance that's actually being used by people that are important to us - the general public is welcome to use that service too, by then.

## What you have done during the weekend

The project came to life during this weekend. From brain storming to conceptualization to coding and deployment. It all happened from Friday 2020-04-24 to Sunday 2020-04-26.

Our achievements and what's left is described in the paragraphs above.

## The solution’s impact to the crisis

At least _we_ will use the application to use it with family and friends. It will certainly help to worry a little less about people that are important to us.

We hope that the general audience will find our contribution useful, too. We're there to help.

## The necessities in order to continue the project

As mentioned above, there's literally tons of work left. We are full of ideas and our TODO lists are even fuller. We got to know each other during the hackathon and we already scheduled time after the event to continue with this project.

However, we all (luckily still) have daylight jobs, so for now it looks like this will stay some kind of freetime project, unless somebody wants to make us a great offer.

## The value of your solution(s) after the crisis

Our service is supposed to help people stay in contact with each other. That is generally a good idea and therefor the service _works quite well_ even if there is no crisis.

## The URL to the prototype [Github, Website,...]

All documentation, concepts and the complete codebase can be found at https://github.com/TheRealWolkenbruch

We will bring live our own _AreYouThere_ installation somewhere on the internet as soon as we feel confident enough to do so. This will most likely happen within the next few weeks.

## The URL to the pitchvideo (Required)

We decided to not provide a video pitch and instead move forward our project technology-wise.

All members of the team have some IT background - video-editing would have been very time-consuming and did not really contribute to the project itself.

We provided everything we could provide within the given time.

## Famous last words

Thank you to all team members, hackathon participants and of course to the organizers & mentors. This has been a great experience and we wish everybody only the best and that we'll make it through this crisis as quickly as possible.

Stay healthy, take care & #flattenthecurve.

-- [Hendrik Bergunde](https://hendrikbergunde.me/) - April 2020
