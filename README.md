<b>How do I invoke a SOAP webservice from curl?</b><br/>

Have the SOAP Request XML in a text file (SOAPRequest.txt)<br/>

Use the below command. <br/>
curl -d @C:\tmp\SOAPRequest.txt -H "SoapAction:http://www.webserviceX.NET/GetQuote" -H "Content-Type:text/xml" -H "charset:utf-8" http://www.webservicex.net/stockquote.asmx

option -H is used to add HTTP header to the request. <br/>
option -d is used to perform HTTP POST<br/>
