# ChatCSV-Streamlit-App
An LLM powered ChatCSV Streamlit app so you can chat with your CSV files.

<h1> How to run the app?</h1>
<p> OpenAI instantly revokes the API key once it detects that the key has been exposed publicly. So, that's the only thing to take care of.</p>
 
 Generate your OpenAI API key here: <a href="https://platform.openai.com/account/api-keys"> Click Here </a>
<br>
<h2> Run locally </h2>
<p> If you are running the app locally, then you can freely use the API key. <br>
  in app.py, line 11: <br>
  
  ```
  
  openai_api_key = 's#-#####################jz'
  
  #can set the API key directly, if running locally.
  
  ```
 
 Else if you want to keep the key private, store it in an environment variable named 'API_KEY' in your OS and then refer the key in app.py by:
 
  ```
  from dotenv import load_dotenv
  load_dotenv()
  openai_api_key = os.getenv("OPENAI_API_KEY")
 
  ```
  
 
  Henceforth make sure to have Streamlit installed in your system. Run the app by:
  
  ```
  git clone https://github.com/AIAnytime/ChatCSV-Streamlit-App.git
  cd ChatCSV-Streamlit-App
  pip install -r requirements.txt
  streamlit run app.py
  
  ```
 <h2> Run on Cloud </h2>
 
 <p> You can also run this app locally on Streamlit Cloud, which is a free Cloud Hosting Service. 
 <br>
 Make a .env  file and store the key as 
 
 ```
 OPENAI_API_KEY='##-###############'
 
 ```
 There's already a .gitignore file with .env mentioned in it. If not, make one. <br>
 Remaining code remains the same.

