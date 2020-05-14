# Pre requirements
Setup Ubuntu ODBC Drivers\FreeTDS
Python 3.6
PIP
Python Virtual Enviroment: 
-- https://realpython.com/python-virtual-environments-a-primer/


# Setup
1. Go in to cloned directory
2. Create Python3 Virtual Enviroment
	python3 -m venv venv
3. Active the Virtaul Enviroment
	python3 -m venv env
	You should see (env) infront of your prompt
4. Install Setup tools and pip
	pip3 install -U setuptools pip3
5. Install the required Python 3 Library's use the list below or use the requirements file
	pip install FastAPI
	pip install Uvicorn
	pip install pydantic
	pip install pyodbc
6. Move or copy config.py.sample to config.py	
7. Run uvicorn web server
    uvicorn api:app --reload --host=0.0.0.0 --port=9000
8. Make sure there are no uvicorn console errors
9. Run some RestAPI Querys to the server
10. Visit the swagger API doc page
    Swagger: http://<server_ip>:9000/docs
    ReDoc: http://<server_ip>:9000/redoc
    OpenAPI: http://<server_ip>:9000/openapi.json
11. Learn more about FastAPI: https://fastapi.tiangolo.com/


