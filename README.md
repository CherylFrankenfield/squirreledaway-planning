# SquirreledAway

##### React / React Native capstone project  

#### By Cheryl Frankenfield, 2/23/18

## Description

_SquirreledAway’s goal is to combat boredom, keep you organized, step-up date night and be your local bucket list/ social events organizer. Have you ever said the phrase, ‘We should do that sometime,’ but then never did? If that sounds like you, check out the SquirreledAway app. It helps you remember the things on your local bucket list, like camping at the folk festival, volunteering at the local beer fest each year, attending roller derby, and more!_

## Setup/Installation Requirements

* Git clone [SqOne - SquirreledAway Repo](https://github.com/CherylFrankenfield/sqOne.git)

Run:
* npm install
* react-native run-ios

Dependencies:
* Emulator for mobile - Expo app or Xcode

## Planning

### 1. Specs
_The app will allow a user to add an event to a master event list._
* _Input: User touches +New and form view is rendered for user's event input._
* _Output: Event details are captured as new entry in master event list._

_The app will allow a user to view the master event list._
* _Input: User touches Events tab (may also just be the home view)._
* _Output: List of master events are displayed in that view._

_The app will allow a user to view a single event._
* _Input: User touches single event displayed on master events lists view._
* _Output: View is rendered to review that event's details._

_The app will allow a user to update a single event._
* _Input: User touches form field and keypad is displayed for editing._
* _Output: User clicks done and new edits are saved to event._

_The app will allow a user to delete a single event._
* _Input: User touches/clicks a delete X or button._
* _Output: Entry is deleted and removed from overall list (future user story here may be an "are you sure?" toaster indicator)._

_The app will allow for events to be saved in database._
* _Input: User adds multiple bucket list items to master list._
* _Output: These are all saved in database and available to view in next session of opening app._

### 2. Future User Stories/Dependencies

1. A user has a specific account login and app allows for multiple users. AuthO and authentication needs to be implemented.
2. A user has a profile page and/or settings functionality with the ability to upload a profile image.
3. A user can search by month for event. Look at UI library for pre-built month UI components.
4. A user can receive notifications of upcoming event(s). Investigate push notification tools for mobile.
5. A user can search by keyword for event. Look into keyword search ability and implement logic. Prebuilt keyword tagging may include: Restaurant, Music, Festival, Sports, Comedy, Arts, Season, Months. Ability for personalization in keywords by user, for example, would include: Mushroom hunting/spots, Camping trips/permits, Bike festivals, etc.
6. Events can have a repeat checkbox to make sure you don’t forget to buy tickets again the following year.
7. Social share component with friends also on the app.
8. Rating system for events/reviews could be hooked up to API (Yelp, other?) if it makes sense.
9. Ticket purchase ability could be hooked up to API (if applicable).
10. Logo, domain and marketing webpage could be designed in React to help promote app.
11. App could have license, T&Cs and privacy statement.
12. App could be deployed to App store.

### 3. UX/UI
* Include UI Library. Options include: Semantic UI, Glamorous, NativeBase.
* Develop custom style using CSS objects and modules with React.
* Main mobile view would contain 5 buttons/icons for:
  1. Account
  2. Search
  3. New
  4. Events List
  5. Calendar View

### 4. Project Planning - Outline (2/23/18)

Routes: /home /new /event

Images:
![UI Sketch](./images/wireframe_1.jpg)

![Components highlighted](/images/wireframe_2.jpg)

![Component Tree](/images/component-tree.jpg)

#### Planning Update (3/2/18)
For the past week, I've reviewed several React Native tutorials (Currency Converter, Egghead.io Notetaker) and spun up projects both with create-react-native-app (using Expo app) and with XCode using react-native cli. I found that create-native-app was far easier to get a project started and exploring React Native, as learning all the dev tools that XCode has to offer would be another task to accomplish in the future. One time-consuming challenge yesterday (using XCode), was realizing that I needed to downgrade Node, after troubleshooting some other fixes that didn't work. All in all, today has run smoother with the goal to rebuild the static web components I did last [Friday's repo here](https://github.com/CherylFrankenfield/squirreledaway-react-web.git) into a mobile component structure [here](https://github.com/CherylFrankenfield/sqOne.git).

My other goals for today/this weekend are to work through my eventual database structure, build out core components, read sections from O'Reilly's "Learning React Native" book, and continue to tackle the React Navigation as that is a key piece to being able to view/test all static components before moving on.

### State Planning (3/2/18)
Please see Component Tree above. I had planned on state living in a Body component previously, but will need to work out the difference between components and screens in mobile / React Native. Since the Header/Footers seem to act more like routes in RN, most likely I will adjust state and place inside common parent -- Home. I plan to use Redux for state management eventually as I'll be using a database to store user info/events.

### File Structure (3/2/18)
![Folders](/images/files.png)

## Known Bugs

_Text ._

## Support and contact details

_If you have any issues, questions, ideas or concerns, please contact me._

## Technologies Used

* React
* React Router (React Navigation Router)
* React Native
* Redux
* Webpack
* Firebase
* Expo App - mobile emulator
* JavaScript
* HTML
* CSS

### License

*MIT*

Copyright (c) 2018 **_Cheryl Frankenfield_**
