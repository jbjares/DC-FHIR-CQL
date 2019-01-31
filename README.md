
#Docker Compose to Intall HAPI FHIR and CQL Ealuation

##If would like to use or test the FHIR Server (HAPI VerionI). So you will probably need the evaluation engine component to perform validations against the CQL syntax. Looking for that this docker-compose gives you the opportunity to quick and easy install as well as put both HAPI FHIR and the CQL Evaluation Engine to run in your own environment, using your properly resources, like data, code system, bundles, or any other type of resources.

##First, you will need to upload some resource data to HAPI FHIR (maybe I can share someone in the next version).
Second the endpoint do query the data using the CQL features (It's already provided), you just need to access the http://localhost:8080/baseDstu3/ to have access to the data service as well as to the terminology URI (Of course, if there are data and any terminology), if you are in doubt please take a look at: https://www.hl7.org/fhir/documentation.html

##Now, if you understood the basics, as well as would like to go forward, looking for creating and executing queries you can send your content for syntax validation through the http://localhost:8082/cql/evaluate. So, if your terminology, data, and query are all well aligned, you will receive an HTTP 200 from this endpoint which means that everything is ok to proceed with the query on FHIR.
so to run the document, please open your terminal (console), use git to clone the project or just download it for some folder and execute this: docker-compose up (in the same folder of the file).

####PS.: There are plans to include new features, applications, some examples using Java, Python or any other language, some data, as well as some scenarios. All advice are very welcome.


###Thanks!!!
