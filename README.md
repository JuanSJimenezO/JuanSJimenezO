<div>
  <h2 align = "center" id = "heading" font-weight =  bold>Hi, I'm Juan Santiago 👋</h2>
  <h4 align="center" id="heading">Data Analyst, Developer and Economist</h4>
</div>


```Python
import json

class Resume():

  def __init__(self, name = "Juan Santiago", last_name = "Jiménez"):
  
    self.code = [
        "Python", "R", "SQL","NoSQL"
        ]
    
    self.ask_me_about = [
        "Data Science", "Machine Learning", "Optimization", "Games Theory"
        ] 
    
    self.knowledge = {

        "Unsupervised Learning" : {
            "topics" : ["PCA", "K-Means", "hierarchical clustering", "KNN"],
            "Frameworks & Libraries" :["scikit-Learn"]
            },

        "Supervised Learning" : {
            "Topics": ["Deep Learning", "NLP",  "Convolutional NN", "Recurrent NN", "LSTM NN",
                       "Multi layer perceptron", "Linear Regression","Support vector machine",
                       "Decision Trees", "ARIMA models"],
            "Frameworks & Libraries": ["TensorFLow","PyTorch", "Scikit-Learn","Keras","statsmodels"]
            },

        "Reinforcement Learning" : {
            "Topics": ["classic control", "Robotics", "Algorithms", "Finance"],
            "Frameworks & Libraries": ["Keras RL", "TensorFlow RL","Stable-baselines"]
            },

        "Optimization" : {
            "Topics": ["Static Optimization", "Dynamic Optimization"],
            "Fraameworks & Libraries": ["Gekko", "Scipy"]
            }
        }

    self.databases = [
        "mongo", "MySql", "sPostgreSQL","Netezza", "SQL Server"
         ]

    self.backend = [
          "Flask", "FastAPI"
           ]

    self.misc = [
          "Spark","DataBricks","Selenium", "BeautifulSoup", "NLTK", "Pandas", "Numpy", "SqlAlchemy", "DASH" 
            ]

    self.architecture = [
          "Web Services", "Lambda (Serverless)"
          ]

    self.cloud_technoliges = [
          "AWS", "Azure"
          ]

    self.learning_goals = [
          "NEAT", "Transformers", "UX", "UI", "JavaScript"
          ]

  def __str__(self):

      consolidated_resume =  {
          "Ask Me About" : self.ask_me_about,
          "Code Knowledge" : self.code,
          "Topics Knowledge" : self.knowledge,
          "Databases Knowledge": self.databases,
          "Backend Knowledge" : self.backend,
          "Architecture Knowledge" : self.architecture,
          "Cloud Knowledge" : self.cloud_technoliges,
          "Miscellaneous" : self.misc,
          "Learning Goals" : self.learning_goals
          }
      return json.dumps(
          consolidated_resume,
          indent = 4
          )
           

print(
    Resume()
    )
 
```



<h2 align = "center" font-weight =  bold> My Projects 💬 </h2>


<h3 font-weight =  bold align = "center"> Optimal Portfolio Delivery Service  💵📈 </h3>
<h3 font-weight =  bold> Topics: </h3>
<p>
  <span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Optimization-black" />
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Financial Markets-critical" />
    </span>    
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Web Service-success" />
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Data Engineering-informational" />
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Web Scraping-blueviolet" />
    </span>
  </span>
</p>

<h3 font-weight =  bold> Stack: </h3>
<p>
  <span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Python-yellow" />
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-MySQL-blue"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-FastAPI-brightgreen" />
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-SQLAlchemy-red"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Pandas-blueviolet"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Numpy-ff69b4"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Scipy-yellowgreen"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Yahoo Finance API-430297"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-Selenium-AAAAAA"/>
    </span>
    <span style = "pading : 2px; display: inline;">
      <img src="https://img.shields.io/badge/-BeautifulSoup-green"/>
    </span>
  </span>
</p>
<br>

<h3 font-weight =  bold> About the project </h3>
<span>
  <b>Portfolio Delivery Service</b> (PDS) is web service offered to minimize the risk-return tradeoff of an investment portfolio. Through an optimization model, based on the 
  <i>Modern Portfolio Theory</i> by Harry Markowitz (1952), and performing built-in customer risk assessment, PDS is capable to give advice about asset allocation and offers a 
  group of custom-made portfolios. Furthermore, the built-in algorithm is more time-stable and scalable than current machine learning models that are input-size and 
  training-sample dependent.  Hence, this project displays how a complex theory-based optimization model could be implemented to put into production and give real life 
  solutions for the clients.
</span> 


  <li>
    <h4 font-weight = bold> 
      <a href = https://github.com/JuanSJimenez2890/Database/tree/main/Yahoo_Finance>
        Yahoo Finance Extraction,Transform, and Load Process
      </a>
    </h4>
    <p>
      The repository contains the data pipeline that was used to update the "asset", "type of asset" and "exchange" tables that were contained in the database. the layers are:
      <ul>
        <li>
          <p>
            <a href = https://github.com/JuanSJimenez2890/Database/tree/main/Yahoo_Finance/Extract>
              <b>Extraction Layer</b>
            </a>
          </p>
          <p>Web Scrapper that mines the  
            <a href = https://finance.yahoo.com/lookup>
            Yahoo Finance symbols list
            </a>
          </p>
        </li>
        <li>
          <p>
            <a href = https://github.com/JuanPChicaC/DataBases/tree/main/ETL/Yahoo%20Finance%20ETL%20Process/Transform>
              <b>Transformation Layer</b>
            </a>
          </p>
          <p> Process that clean and normalize the information that comes from <b>Yahoo Finance</b> in order to fit into the database tables</p>
        </li>
        <li>
          <p>
            <a href = https://github.com/JuanPChicaC/DataBases/tree/main/ETL/Yahoo%20Finance%20ETL%20Process/Load>
              <b>Load Layer</b>
            </a>          
          </p>
          <p>In this step, the records are pushed into the 
            <a href = https://github.com/JuanPChicaC/DataBases/tree/main/SQL/Portfolio%20Optimization%20DataBase>
              Portfolio Optimization DataBase
            </a>
          </p>
        </li>
    </ul>
    </p>
  </li>

</ul>
