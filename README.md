# LinkedIn Web Scraper

This is a LinkedIn Python Web Scraper for companies. The script fully simulate a human activity (using [Selenium](https://selenium-python.readthedocs.io) library) in order to get data from LinkedIn web pages. The purpose is store data from companies of a certain zone, such as:

- Name 
- Overview/Description
- Size
- Website link
- Industry
- etc.

After collected the above information, these will be stored into an `.xls` file.


### Disclaimer

Any actions and or activities related to the material contained within this repo is solely your responsibility. The misuse of the information in this repo can result in criminal charges brought against the company in question. The author will not be held responsible in the event any criminal charges be brought against any individuals misusing the information in this repo to break the law.

As written in [Linkedin User Agreement]: **you agree you will not use** [...] any bots or other automated methods to access the Services, add or download contacts, send or redirect messages.
   
### Terms And Conditions

- I do not promote, encourage, support or excite any illegal activity or hacking without written permission in general. The repo and author of the repo is no way responsible for any misuse of the information.
- "linkedin-web-scraper" is just a terms that represents the name of the repo and is not a repo that provides any illegal information.
- This repo is totally meant for providing information on Computer Software, Computer Programming and other related topics.
- The Software's and Scripts provided by the repo should only be used for education purposes. The repo or the author can not be held responsible for the misuse of them by the users.
- I am not responsible for any direct or indirect damage caused due to the usage of the code provided on this site. All the information provided on this repo are for educational purposes only.

### Demo

[![Watch the video](https://img.youtube.com/vi/TKkJEo-4NTg/maxresdefault.jpg)](https://youtu.be/TKkJEo-4NTg)

# Table of Contents

- [Usage](#usage)
- [Troubleshooting](#troubleshooting)
- [Resources](#resources)

# Usage

1. Clone project

       git clone https://github.com/J4NN0/linkedin-web-scraper.git
       cd linkedin-web-scraper
    
2. Install requirements

       pip install -r requirements.txt
    
3. Download the web driver you prefer and put it inside project folder:
    
    - [Firefox](https://github.com/mozilla/geckodriver/releases)
    - [Chrome](https://chromedriver.chromium.org/downloads)

4. Set missing configs in `config.ini`:

   - LinkedIn credentials i.e., `EMAIL` and `PASSWORD`.
   - The `WEBDRIVER` (downloaded on step `3`).
   - And `CITY` from which companies have to be fetched.
   
   Note that also others kind of parameters can be set.

5. Run script

       python3 main.py

   Data will be store into `companies.xlsx` file.

# Troubleshooting

- It could happen that, after the logging phase, LinkedIn could ask you to perform some actions/operations (e.g. "I'm not a robot", etc.) instead of redirecting you to the feed (https://www.linkedin.com/feed/) page. 

    In this case:
    
    1. Stop the script.
    2. Log in with a browser in your account.
    3. Skip the required actions.
    4. Re-run the code.

- If you face some issues using `Python 3.9` (e.g. on installing dependencies), please try with `Pyton 3.7` or below (but not earlier than version `Python 3.0`).

# Resources

- [Selenium](https://selenium-python.readthedocs.io/installation.html)
- [Chrome Webdriver](https://chromedriver.chromium.org/downloads)
- [Firefox Webdriver](https://github.com/mozilla/geckodriver/releases)
- [Scrapy](https://docs.scrapy.org/en/latest/intro/tutorial.html)
