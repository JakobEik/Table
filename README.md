# Table

# Setup
In order to run our application you have to pip install requests. Some of the imported modules might need a newer version of Python. The program has been made and tested with Python 3.8 so if we can’t guarantee that it will work for older versions .
To setup the application you will need Apache Jena Fuseki server. Once the server is running, upload the shapes.owl ontology to the server. Then unzip and extract all from the zip file and save it to a preferred location.

The website is written in HTML and when a user submits parameters for input, a path will be generated in python. The script extract the parameters and update the Fuseki server using SPARQL queries. After updating the database a GET request is sent to extract the input values from the server, and a new file DFA file is created with the input values as parameters for the table. If there already exist a DFA file it will be overwritten.
