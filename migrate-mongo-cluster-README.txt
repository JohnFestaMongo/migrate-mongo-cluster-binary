The migrate-mongo-cluster jar file was built from the "pete" branch of:
    https://github.com/sarjarapu/migrate-mongo-cluster

Environment
    Built with JDK 11.0.2
    This same binary has been run successfully against a 60TB sharded cluster running under OpenJDK on ubuntu.

Preconditions
    All databases, collections and indexes should be created before running the tool.
    Execute migrate-mongo-cluster-precreate.js to do this

Commandline Help
    java -jar target/migrate-mongo-cluster-1.0-SNAPSHOT-jar-with-dependencies.jar -h

Usage
    Use the Mongo Shell to execute migrate-mongo-cluster-precreate.js
    Point one copy of the migration utility at a mongoD of each shard.
    Point each running copy of the migration utility at the mongoS of the destination.
