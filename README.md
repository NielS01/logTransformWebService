# logTransformWebService
Mule ESB project demonstrates how to log the requests and responses to a web service
without altering the target web service. 

Logging and transformation is done by proxying the web service within the ESB.

This  project provides 2 proxy endpoints (port 7081 & 7082) to the same web soap service:
* Endpoint one logs the request/response to a local folder (say c:\temp\muleESB) as well as transform the XML response to JSON
* The second endpoint merely logs the request and returns the XML response.

Note some configuration is needed to point this to your target SOAP service (in the logtransformservice.xml file, search for
anything prefixed with 'XXX_' :-)
