title:                  Conversations: Find the dialog
description:            Use react to build a messaging front end  
duration:               7 hours
skill_level:            Advanced  
core_concepts:          React, Flux, Babel, Webpack, socket.io
prerequisite_concepts:  CommonJS, npm

slug:                   chat-react
tags:                   React, Node
date_implemented:       Jul 1, 2015

## Overview
The NSA is reading everyone's messages and invading everyone's privacy.  In response to the NSA, your company has built an encrypted messaging API, and you need to build a new frontend for it.  

### Conversation
The most important component is the conversation component.  This will allow users to send messages and display the messages.  Conversations will only have two users and messages between each user will be displayed in ascending order by timestamp with the latest messages on the bottom.

### Conversation List
The application should be able to list all of the conversations you've had with other people.  This list of conversations should be sorted in descending order where the conversation with the latest message is shown on top.


## Milestone 1
- Create a blank application using Babel and Webpack.  Make sure there is an index.html file that loads the compiled JavaScript.
- Write a react component that displays a textarea to accept messages and a component that renders the messages.  These two components should be wrapped in a single component and communicate to each other using the flux architecture.  There should be an action dispatched from the form component which updates the store which updates the state of the conversation  component.

## Milestone 2
- Create a conversation list component to list each conversation as a single entity, which should be another component called a conversation list item.  The conversation list item will show the username and last message so that it can easily be identified.  This list will be sorted in descending order with the most recent thread on top.
- When messages are added to a conversation, the conversation list should reorder itself.  Using the flux architecture, set up the conversation list component to listen to changes in the store so that it can reorder the conversation list items when a new message is added.
- Since users only want to check conversations when they get new messages, add a "new message" indicator to the conversation component in the conversation list component.  When a user clicks on the conversation, it should be marked as read and the indicator removed.

## Milestone 3
- Create a page for the user to enter a username.  Save the username in a user store, but do not persist the username to local storage.  Keeping the username in memory will allow us to log in as multiple users.  The application should inspect the user store to see if there is a username.  If there is no username, display the login component, else render the conversations and messages.
- Use socket.io to emit messages to the server from the message store and to receive for the the message store reieve messages from the server.  The conversation list component and conversation component should have listeners on the message store in order to be updated with the latest messages.

## Resources
- [Getting Started with Webpack](http://webpack.github.io/docs/tutorials/getting-started/)
- [Babel with Webpack](https://babeljs.io/docs/setup/#webpack)
- [Flux Overview](https://facebook.github.io/flux/docs/overview.html)
- [Actions and the Dispatcher](https://facebook.github.io/react/blog/2014/07/30/flux-actions-and-the-dispatcher.html)
- [Partial Solution](https://github.com/facebook/flux/tree/master/examples/flux-chat)
- [socket.io chat](https://github.com/Automattic/socket.io/tree/master/examples/chat)