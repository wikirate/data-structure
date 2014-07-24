data-structure
==============

Define the notation and structure for communication between CERTH's software and WAGN


### What's needed from WAGN

* A method to push new sources to CERTH (At the moment we pull the list "by hand" or we can have a cronjob for this)
* A method to get the list of topics which includes the list of related companies for each topics (and probably a push notification when new topic is added)
* A method to get the list of companies which includes the list of related topics for each topics(and probably a push notification when new company is added)

(Pushing new topics/companies/sources, etc are needed so as to update our collection(s) -> fetching, indexing, etc)

### When to invoke CERTH services
1) When user adds a new claim and enters the title
  *  Input: title (or to be more precisely: a set of keywords --> we transform title to keywords after all)
  *  Output: a list of "links" relevant to the input consisting of: id, URL, title, array of related to the URL images, name of wikirate source if it's an internal "link"

2) When user adds a new claim and enters a new source (URL)
  *  Input: any valid URL
  *  Output: a list of "links" relevant to the input consisting of: id, URL, title, array of related to the URL images, name of wikirate source if it's an internal "link"

3) When user adds a new claim and enters a set of topics and/or set of companies
  * to be further discussed internally (CERTH) and propose a solution


## Testing tools
* https://github.com/wordnik/swagger-ui (setup a swagger for your convenience if needed)
* http://restclient.net/ (as FF extension)
* http://www.jsoneditoronline.org/
* any REST client you like :)
