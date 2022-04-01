# Data analysis
- Document here the project: 
  stock_backend
  
- Description: 
  Project Description
  
- Data Source: 
  ~~API Call Via [yfinance](https://pypi.org/project/yfinance/) (Open-Source Tool that access [yahoo finance API](https://python-yahoofinance.readthedocs.io/en/latest/api.html))~~
  
  Web Crawl on [KRX](https://global.krx.co.kr/contents/GLB/03/0308/0308010000/GLB0308010000.jsp), for stock codes
  
  API Call Via [iexcloud](https://iexcloud.io/docs/api/) for Daily Data for the model
  
- Type of analysis:
  

# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
make clean install test
```

Check for stock_backend in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/stock_backend`
- Then populate it:

```bash
##   e.g. if group is "{group}" and project_name is "stock_backend"
git remote add origin git@github.com:{group}/stock_backend.git
git push -u origin master
git push -u origin --tags
```

Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
stock_backend-run
```

# Install

Go to `https://github.com/{group}/stock_backend` to see the project, manage issues,
setup you SSH public key, ...

Create a python3 virtualenv and activate it:

```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:

```bash
git clone git@github.com:{group}/stock_backend.git
cd stock_backend
pip install -r requirements.txt
make clean install test                # install and test
```
Functional test with a script:

```bash
cd
mkdir tmp
cd tmp
stock_backend-run
```

# References

- [Fear and Greed Index](https://www.liberatedstocktrader.com/fear-and-greed-index/) (Reference only)
  **Following Resource is used as a reference for buy and selling of stock**
- [An NLP and LSTM Based Stock Prediction and Recommender System for KOSDAQ and KOSPI](https://www.researchgate.net/publication/349071337_An_NLP_and_LSTM_Based_Stock_Prediction_and_Recommender_System_for_KOSDAQ_and_KOSPI)
- [KRX](https://global.krx.co.kr/contents/GLB/03/0308/0308010000/GLB0308010000.jsp)
