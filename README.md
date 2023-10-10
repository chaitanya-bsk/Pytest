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
Pytest/ 
├── assertionhelpers/ # Test data 
			├──base 
			├──contact
├── clients/ # Test scripts 
			├──base	
├── configs/ # Cypress plugins 
├── constants/ # fetching the constant data 
├── datahelper/ # helps in fetching the data 
├── executors/ # execute the api by sending it to respective service 
├── services/ # Cypress plugins 
		├──base
		├──contact	
├── templates/ # JSON FILES  
├── tests/ # tests  


# Report generation - 
pip install pytest-html
Once test is completed view it in html location ( /report.html )
