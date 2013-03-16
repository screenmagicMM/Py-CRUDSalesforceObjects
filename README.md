
PushToSF
========

We were exploring our ways to access, add and modify Salesforce Standard and Custom objects. We wanted to write python module so that we could do the operations from command line.

There are two ways to achieve this -  

_ **Using WebService:**
                For WS, we chose - salesforce-python-toolkit from [here][1].
                This toolkit uses SOAP api to make various operations like create, delete, update, upsert, etc. using WSDL files provided by Salesforce. You can see for all the possible operations on SF objects in wsdl files. Calling a webservice with SOAP will need the actual credentials. As we had encrypted credentials which were encrypted using CodeIgniter's Encrypt library. So we wrote a module - Decrypt to decode them.

_ **Using OAuth:**
                 They had explained things really well [here][2]. But the API was in Java. We started searching for a python API for for Salesforce objects. There was none. In fact I think nobody had written it using python. So instead of searching more, we wrote a module of our own.

  [1]: http://code.google.com/p/salesforce-python-toolkit/ 
  [2]: http://www.salesforce.com/us/developer/docs/api_rest/api_rest.pdf 
