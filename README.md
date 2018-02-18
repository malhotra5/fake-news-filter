# Fake News Filter 
An application to detect fake and untrustworthy websites using python
## Getting started
Run the application by running the file Main_App.pyw
### Prerequisites
* pyqt4 (gui toolkit)
* sqlite3 (database management system)
* bs4 (beautiful soup, parsing html and xml documents)
* urllib 
* sys
### Installation
All wheel files for python3 modules above can be found at https://www.lfd.uci.edu/~gohlke/pythonlibs/ \
Once the wheel files are downloaded, run the command below for every wheel file. 

    pip install WheelFileName.whl 

Alternative 
    
    pip install bs4 
    pip install sqlite3 
    pip install pyqt4 
    
## Running the application
Run the file Main_App.pyw
## How it works
Once the url is entered, the application formats it. \
Then, the application uses a database of fake and real websites. If the url is found in the database, it outputs the result accordingly (either fake or real).\
If the url does not exist in the database, the application uses bs4 to download the html code for the entered url. \
The application gets all the ``` <a> ``` tags. This is to get all the references (urls) for the website. \
The references are cross checked in the fake url database. \
If any of the references are fake, the url entered is appended to the fake url database. The application returns fake as it's output. \
If none of the references are fake, the application's output states that it can't tell whether the url entered is fake or real.  

## Results
How the application looks \
![GitHub Logo](/Results/options.jpg)

Application outputs \
![GitHub Logo](/Results/RealOutput.jpg)
![GitHub Logo](/Results/FakeOutput.jpg)

## Built with
* Python3
* DB browser for sqlite (for visualizing the database)
* Exel (for making list of fake and real website)
## Acknowledgments
All my team members for the hackathon in which this project was built.



