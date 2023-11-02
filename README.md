Flutternetes is an open-source bundle of tools and guidelines and best practices to created flutter apps using the micro-service strategy

# What it is right now

right now it is just an example application built using the micro-service strategy and the crusader architecture(i have named the architecture cursader because i love the original Stronghold Crusader game :D ). the example project is called cats

# 🎯 Goals

1 - complete the cli to automate the creation and maintaining the micro-services ❌

2 - create a cli for publishing package to artifact management platforms like cloudsmith.com ❌

# The cursader architecture

it is an architecture designed to create flutter micro service application.

it has 4 types of micro service:

1 - the endpoint micro service: the flutter app that containes all the other microservices and will be used to publish the app

2 - the visible micro services: these are flutter plugin projects that are visible meaning that they have an example app project that can be run on a device

3 - the runner micro service: it is a flutter package and it is the runner for the visible micro services

4 - the invisible micro service: theses are flutter package projects and they provide service like localization or routing to other microservice and they can not be run.


here is the dependecy graph of the cats project:






