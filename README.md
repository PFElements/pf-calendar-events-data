# \<pf-calendar-events-data\>

# pf-elements
A Polymer 2.0 based collection of reusable web components [![Join the chat at https://gitter.im/pf-elements/Lobby](https://badges.gitter.im/pf-elements/Lobby.svg)](https://gitter.im/pf-elements/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# pf-calendar-events-data

An Advanced Polymer 2.0 based custom elements to get the calendar events, appointments, meetings data from Firebase. To be used in conjunction with pf-calendar-events element


| Element Name | Latest Version (Bower) | Npm version  | Build Status |
|--------------|------------------------|--------------|--------------|
| [pf-calendar-events-data](https://github.com/PFElements/pf-calendar-events-data) | [![GitHub version](https://badge.fury.io/gh/PFElements%2Fpf-calendar-events-data.svg)](https://badge.fury.io/gh/PFElements%2Fpf-calendar-events-data) | [![npm version](https://badge.fury.io/js/pf-calendar-events-data.svg)](https://www.npmjs.com/package/pf-calendar-events-data) |[![Build Status](https://travis-ci.org/PFElements/pf-calendar-events-data.svg?branch=master)](https://travis-ci.org/PFElements/pf-calendar-events-data) | 


[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/owner/my-element)

## Demo
[Click here for docs & demo](https://github.com/PFElements/pf-calendar-events-data/blob/master/demo/index.html)


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.


## Learn more

See the list of elements, demos, and documentation by browsing this collection on webcomponents.org:

### [Take me to webcomponents.org ›](https://www.webcomponents.org/element/PFElements/pf-calendar-events-data)

### Methods
The following methods are available for crude events operation:

Methods                                 | Description                           
----------------------------------------|--------------------------
`addEvent(event)`                       |  Take event object and add as a new Event, meeting or reminder into firebase 
`updateEvent(key,event)`                |  Take firebase data ref key and updated event object , update the given ref key node                          
`deleteEvent(key)`                      |  Take record ref key and delete that event                    
            



# Example

```html

     <firebase-app
                  name="pf-calendar-firebase"
                  api-key="AIzaSyBOML3Qc_rtqDeVAr2ous6Z8-E1FDqH4CI"
                  auth-domain="pf-calendar-firebase.firebaseapp.com"
                  database-url="https://pf-calendar-firebase.firebaseio.com">
          </firebase-app>
          <pf-calendar-events-data
                  databasename="pf-calendar-firebase"
                  databasepath="testdata"
                  eventsData="{{results}}"
                  filterAttr="color"
                  filterValue="green"></pf-calendar-events-data>
```
-> Replace firebase-app with yours 




## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## Contributing

Comments, questions, suggestions, issues, and pull requests are all welcome.


### Get in touch with the team

Joing us at [![Join the chat at https://gitter.im/pf-elements/Lobby](https://badges.gitter.im/pf-elements/Lobby.svg)](https://gitter.im/pf-elements/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

- [Twitter](<a href="https://twitter.com/polymerio" class="twitter-follow-button" data-show-count="false">Follow @polymerio</a>)
- [Facebook] (https://www.facebook.com/polymerjs)
- [Google+] (https://plus.google.com/116168214823506639166) 
- [YouTube] (https://www.youtube.com/channel/UCDKqvDyAn_QTBvCPvrZKTkw) 

### Some ways to help:

- **Test the elements and provide feedback**: We would love to hear your feedback on anything related to the elements, like features, API and design. The best way to start is by trying them out. And to get a quick response, either drop a question/comment on the chat or open an issue in GitHub.
- **Report bugs**: File issues for the elements in their respective GitHub projects.
- **Send pull requests**: If you want to contribute code, check out the development instructions below.

We encourage you to read the [contribution instructions by GitHub](https://guides.github.com/activities/contributing-to-open-source/#contributing) also.

## License

MIT License
