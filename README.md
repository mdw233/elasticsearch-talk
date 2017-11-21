# Elasticsearch Talk
These are slides (using [reveal.js](https://github.com/hakimel/reveal.js/)) to be used for an Elasticsearch intro talk.
# View Presentation
Open `index.html` with any browser and use the left/right arrows to navigate.

Or visit: https://mdw233.github.io/elasticsearch-talk
# When / Who?
The talk was given on 1/23/2017 to the University of Pittsburgh Computer Science club.
# Why?
Why not.
# Data
This talk assumes that you're going to create an index named `pitt_talk` and a type named `review`.  As such, all commands and examples will be written using those values.  
## Postman Data
The `postman-collections` folder has 2 collections you can import into Postman and run during the live demo.  Please note - the url in the `IC Staging ES.postman_collection` isn't real - it's just a hosts entry for the purposes of this talk.  The data in that collection is data used by [ImagineCareers.com](https://imaginecareers.com) staging environment.
Two of the reviews are added via commands in `ES Pitt.postman_collection`.  The remaining data is in the `reviews` folders.
## Review Data
The review data for this talk is in the `reviews` directory.  You can easily upload all of those files via the following command (assuming you have Elasticsearch installed at localhost:9200`):

`find "{path to this workspace on your computer}\revealjs-elasticsearch\reviews" -type f -exec curl -XPOST http://localhost:9200/pitt_talk/review --data-binary "@{}" \;`

`
