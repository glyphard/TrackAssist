# TrackAssist
A FogBugz API wrapper and rudimentary desktop client.

# What's Included
The bulk of the API is in FogBugzApiWrapper project. The rest of it is a test-bed and some experimental work around creating a desktop client with pluggable widgets.

# What does it do?
Not too much, yet. But it does deserialize FogBugz XML responses into real objects you can mess with. Most, if not all, of this is likely to change soon (and a lot) as there are already a few decisions that I'm not thrilled about.

But if you want to pull some basic data from FogBugz and operate on it (the API wrapper is primarily geared toward read access right now), this may be just the thing for you.

# How do I use it?
There are a couple of convenience methods for listing cases, users, milestones, and timesheet entries (intervals). If you want something more customized, most of the API is covered by creating your own GenericFogBugzRequest object, specifying your command and a collection of GenericRequestArgument objects.

# What's coming?
I intend to add request validation, so you can get feedback on when you supply invalid arguments as well as some specialized ways to generate requests (so that you know you're generating a valid request before submission).

The goal is to create a wrapper that can not only read from FogBugz, but also write data back in a convenient way. (Think, pull data, modify object, save it back.)

The secondary goal is to have a desktop client that helps make managing certain aspects of time tracking and project management a little easier. For instance, if you want to be able to break down information in a graph that shows time entry by user by day, this may be the tool for you. It may not be there yet--but that's where I want to take it.
