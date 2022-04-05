![GitHub Repo commit](https://img.shields.io/github/last-commit/SimonMikoda/VS-code)
## Amazing Hello World App

1. setting up virtual python env:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

2. Installing the dependencies:

   ```bash
   pip install -r requirements.txt;
   pip install -r test_requirements.txt;
   ``` 

3. Checking if the app works use `curl` to call the app web api:

   ```bash
   PYTHONPATH=. FLASK_APP=hello_world flask run
   ```

   ```bash
   curl 127.0.0.1:5000
   ```

   ```bash
   curl 127.0.0.1:5000/outputs
   ```

   ```bash
   curl '127.0.0.1:5000/?output=json'
   ```

3. Testing the code:

   ```bash
   PYTHONPATH=. py.test  --verbose -s
   ```

4. Linting our code:

   ```bash
   flake8 hello_world test main.py
   ```

5. Place for notes:

   ```bash
   To check if the code works using heroku, the link:
   https://safe-wildwood-41309.herokuapp.com
   
   We can use both Heroku and Docker for testing
   ```

