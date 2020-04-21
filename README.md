# elasticsearch-nest-webapi-angularjs (.Net4.6.2)
Introduction to Elasticsearch 7.5.2 with NEST, ASP.NET Web API 2 and AngularJS

##Installation

* Install Elasticsearch 7.5.2 from https://www.elastic.co/downloads/past-releases/elasticsearch-7-5-2
* Ensure Elasticsearch is listening on http://localhost:9200/ 

##Download test data

* Download test data from https://archive.org/download/stackexchange,
* or Download meta.stackoverflow.com.7z from https://tejp.de/files/so/dbdump/stackexchange-export-2011-09-01/
* Unzip the archive and copy the `Posts.xml` file to the `data` folder.

* https://meta.stackexchange.com/questions/198915/is-there-a-direct-download-link-with-a-raw-data-dump-of-stack-overflow-not-a-t
* https://meta.stackoverflow.com/questions/295508/download-stack-overflow-database
* https://www.brentozar.com/archive/2015/10/how-to-download-the-stack-overflow-database-via-bittorrent/
* 
##Create the index

* Open the solution in Visual Studio 2019, select Restore NuGet packages and rebuild the solution.
* Make a GET request to https://localhost:44365/api/index?fileName=posts.xml&maxItems=10000

##Run the application
* Debug or Start without debugging to run the Web API in IIS Express.
* Browse to https://localhost:44365/index.html
