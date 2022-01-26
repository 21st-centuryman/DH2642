# Bug-Tracker

Link to site: https://bug-tracker-7979b.web.app/

Bug-Tracker is an app which you can use to track your projects' bugs and issues. Our intention is to give developers a quick overview of
everything that needs to be solved, the source of the issue, who in your project group is assigned to solving said issue, and so on.

This is then combined with a sort of bug bounty hunting system in which you get points for solving an issue, meaning you can level up your account.

...
# Tutorial

To start using bug tracker you will have to set up an account by sign up on the first login page.

You will now be redirrected to the home view. To add projects to your feed. Press the searchbar on the top left and add your github projects you want to work on.

Certify that the information and the project you have selected is the one you want to work on.

Now you have the ability to delete your project off your feed, copy the ssh or http key to your clipboard, or press on the card to start working on bug tracking.

Now you are in the ticket page. Here you are able to add tickets by pressing the add ticket button in the top left. This will prompt you to add a title, priority, description, and whom you are assigning this ticket to.

Each ticket has 4 states, "To-do" (tickets which have not yet started work on), "in-progress", "done" (which are both self explanatory), and lastly "on hold" (for users which have tickets on higher priority but wants to save this ticket for themselves at a later date.)

## Current Progress

So far we've started implementing views and the project board model, the login screen, home screen and DOM routing. In other words, mostly the visuals.
We have some basic css for the board but plan on converting to Semantic-UI later.

## Functionality

- Sign-up and Login/Logout
- Search for and join a public Github project
- Create bug tickets
- Collborate with other developers
- Retrieve SSH-links to github repos.

## Installation

A step by step series of examples that tell you how to get a development enviorment running

Open the directory for **Bug-tracker** and install all modules

```
npm install
```

## Running Application Locally

When all the modules are installed you have to ask one of the authors of the project for a `firebaseConfig.js`-file. Which should later on be pasted in `src/api` in project-directory.

To run the application locally in a development-enviorment. Run:

```
npm run start
```

To start the application on port `3000`.

And to create an optimized production-build. Run:

```
npm run build
```

## Future Plans

We have thought about more quality of life features such as toggling on and off to be able to filter between the diffrent status of the ticket life cyckel i.e:

- Todo
- In Progress
- Done

More over maybe better sorting in regard for priorities, and even some more functionality in the Edit ticket window such us add code snippets to furthurmore clerify readability.

## File Structure

First off, the project has been built using create-react App, which means we have some default files included.

- **.firebase** and any file following the pattern 'firebase[.*]' is related to firebase deployment.

The public directory contains mostly auto-generated files along with some logo png's.

### src

The **src** directory contains all source files.

### Sub-directories

- **api** handles api calls and functionality pertaining to firebase and persistance.
- **core** contains our models for 'boards', users and 'tickets'.
- **hooks** include various custom react hooks.
- **images** is our iamge folder.
- **localization** contains DOM-routing routes and group member information.
- **pages** contains page information.
- **presenters** handles all of our presenters.
- **reducers** contains files for handling Redux states.
- **store** includes the Redux store interface.
- **styles** includes all .css files with the exception of the index file.
- **utils** contains the utility functions.
- **views** handles all views.

- **index.js** and **reportWebVitals.js** are auto-generated by react.