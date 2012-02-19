Flavors
========

This is an entry for the Neo4j Heroku Challenge(http://neo4j-challenge.herokuapp.com/) and is a template for Grails with Neo4j and D3.js web applications.
Inspired by The Flavor Bible by Karen Page and Andrew Dornenburg, this app models flavor affinity between various ingredients in a graph and demonstrates features the Neo4J REST API.

Demo:

Blog posts with more information:

If you like this app, please rate it on Gensen ()

Deploying Locally
=================
* Set up grails
* Set up neo4J
* > git clone git@github.com:luanne/flavorwocky.git
* Edit flavorwocky/grails-app/conf/Config.groovy and point neo4j.rest.serverendpoint to your local neo4j server e.g. "http://localhost:7474/db/data"
* Make sure your local neo4j server is running
* >cd flavorwocky
* >grails run-app
* Launch the app in your browser (e.g. http://localhost:8080/flavorwocky/)


Deploying on Heroku
===================
* git clone git@github.com:luanne/flavorwocky.git
* cd flavorwocky
* heroku login
* heroku create --stack cedar
* heroku addons:add neo4j
* heroku addons:open neo4j
* Edit flavorwocky/grails-app/conf/Config.groovy and point neo4j.rest.serverendpoint to your local neo4j server e.g. "http://localhost:7474/db/data"
* git push heroku master
* Go to your browser and try it out!
