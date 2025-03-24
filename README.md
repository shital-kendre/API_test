#Flask API to trigger Concurrent API calls based on timestamps

#Explaination:
This Project creates a Flask based API that accepts a list of timestamps, triggers concurrent API calls to 'ifconfig.co' and logs the results.
It handles duplicate timestamps concurrently, used modular functions, and includes errror handling.

##How to execute the script##

1. Clone the repository
   use github

2. create and active virtual environment
3. Install dependencies
4. run flask server
5. make API requests

##How the script is structured##
1. Main components
   The project contains main files like:
   app.py
   README.md
   requirements.txt
   config.py
   tests/
2. File Details
   app.py: Conatins Flask API implementation
   
   requiremenst.txt - List of python dependencies required to run project

   test:
   include unit and integration test

   config :
   configuration files

   ## Key Design decision##
   1. Concurrency and multithreading
     To handle API calls used multithreading
  2. Modular Design
     Divided script into :-
     call_api - Makes single API call
     schedule_api_calls - Handles multithreading and concurrent execution
     log_result - Logs success or failure of each API call
  3. Error handling and logging
     Clear distinction between success and failure
  4. Scalability
     used multithreading
  5 Configuration Flexibility
    Project structure includes /config folder for easy modification 
