Two DevOps engineers, Alice and Bob, walk into a bar.  Alice says to Bob: "How many MongoDB instances does it take to ensure that your data is replicated?".  Bob replies: "A minimum of three.  And data loss is not laughing matter."

Okay, so DevOps engineers aren't renowned for their jokes.  But in this project you will be heeding Bob's advice, and setting up a MongoDB replica set so that your data is replicated across multiple servers.

# Milestones

## Milestone 1: Set up a replica set

To complete this milestone you should start three instances of `mongod`, and make them run as a replica set.  Working on the assumption that you don't have three separate machines to run your instances on, you will need to run each instance on a different port (set upsing the `--port` option), and with a different data directory (set using the `--dbpath` option).

Use the [`rs.status()` method](http://docs.mongodb.org/manual/reference/method/rs.status/) to make sure that all three nodes are running as part of the set, with a single primary and two secondaries.

## Milestone 2: Test out the behavior

In this milestone you will be exploring how the replica set works.  To complete the milestone you should:

* Use the `mongo` shell connected to the primary node to add some documents to a new collection.
* Query the collection to make sure that the documents got added successfully.
* Try querying the collection from a shell connected to one of the secondary nodes.  What do you see?
* Simulate the failure of the primary node by halting the `mongod` instance.  Check `res.status()` to see what has happened to the node configuration.
* Make sure that you can still query the documents.  This will show that they have been replicated across the instances.
* Bring the old primary server back up.  What does `res.status()` tell you?

## Milestone 3: Backup and restore

All the replication in the world won't save you from a sudden outbreak of [fat finger syndrome](https://en.wikipedia.org/wiki/Typographical_error) when administering the database.  So to complete this milestone you should:

* Use `mongodump` to create a complete backup of the database.
* Delete all of the documents in the database.
* Use `mongorestore` to restore the database from your backup.
* Query the database to make sure that all of your documents were restored.

# Resources

* The [MongoDB replication introduction](http://docs.mongodb.org/manual/core/replication-introduction/) introduces the key concepts behind a replication system.
* [This tutorial](http://docs.mongodb.org/manual/tutorial/deploy-replica-set/) shows how to deploy a replica set across three different machines.
* [This guide](http://docs.mongodb.org/manual/tutorial/backup-and-restore-tools/) shows you how to use the `mongodump` and `mongorestore` tools to backup and restore a Mongo database.
* [This article](http://spf13.com/post/backups-replication-and-disaster-recovery) discusses the different problems which can cause to data loss, and looks at how the configuration of your databases can help to mitigate this.

