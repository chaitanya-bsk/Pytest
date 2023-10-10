# Pytest

# Setup 
Prerequisites
Install python - Python 3.11.5
Install pip - pip 23.2.1
Install pytest - pytest 7.4.2

# .ENV FILE 
This file or environment variables are typically used for configuring and storing sensitive information or configuration settings that your tests or applications need.
We have stored API KEY and API ID in this path and later fetched in out tests



# How to execute test-
run tests with specific markers as follows ->  pytest -m smoke
Run all the tests -> pytest 


# Folder Structure- 
This contains the structure of the framework. 
Services here are - ex- call / user/ name / contact / each set of API collections. This helps in easy segregation 
- assertionhelpers are used to assert respective services
- datahelper - helps in fetching data 
- clients - will call the API request
- executor - it will call the respective service API 
- templates - this will contain schema , some test data
- tests - will have test scenarios for each service - ex: all contact related test cases can be written in contact.py. Any common test cases can be written in base.py

- Pytest/
  - assertionhelpers/
    - base.py
    - contact.py/
  - clients/
    - base.py
  - configs/
  - constants/
  - datahelper
  - executors/
  - services/
    - base.py
    - contact.py/
  - templates
  - tests
    - base.py
    - contact.py/
     	- contactsearch_test



# Report generation - 
pip install pytest-html
Once test is completed view it in html location ( /report.html )
