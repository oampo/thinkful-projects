## Build

Thinkr is the hot new social network which lets you tell the world what you are thinking in Thoughts: messages made up of four or less characters.  In this project you will be building the API which allows users to create, retrieve, update, and delete thoughts, and storing them in a MongoDB database.

## Milestones

### Milestone 1: Set up the schema

Use Mongoose to create a schema and a model for Thought objects.  Thought objects should contain a string which represents the username of the user who added the thought, and a string containing the content of the Thought.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/e292f63344e14a1ba97a).

### Milestone 2: Creating Thoughts

Set up a simple Express app, and add a POST endpoint for creating new Thoughts at `/thoughts/:user`.  The endpoint should take JSON data containing the content of the thought, and add this to the MongoDB database.

Test out your endpoint using cURL, and make sure that the Thought has been added to the database using the MongoDB Shell.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/4a5f3358f432c24996ac).

### Milestone 3: Retrieving Thoughts

Add two new GET endpoints which allow you to retrieve a list of a user's thoughts at `/thoughts/:user`, and a single thought at `/thoughts/:user/:id`.  Test out your endpoints by using cURL to retrieve the thought which you added in Milestone 2.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/74d85a506bbc6431ae8d).

### Milestone 4: Updating Thoughts

Add a PUT endpoint which allows you to edit a Thought at `/thoughts/:user/:id`.  Use this to edit the thought which you added in Milestone 2, then use one of the retrieval endpoints to make sure that the Thought has been edited successfully.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/3599b28bfdf1a6bbdd35).

### Milestone 5: Deleting Thoughts

Add a DELETE endpoint which allows you to delete a Thought at `/thoughts/:user/:id`.  Use this to delete the thought which you added in Milestone 2, then use one of the retrieval endpoints to make sure that the Thought no longer exists.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/026a4ee234fb9e50fea6).
