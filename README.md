# Web-Scrapping
---  
The outcome of this repository is to scrape data about various Indian movie celebrities. The information I have extracted for each actor include - _Name_, _Image_, _Age_, _Height_, _Description_  

#### Modules used  
---  
* I have used the popular **BeautifulSoup** library for the scrapping purpose, along with other helping library **requests**.  

* I have also used **Pandas**, to generate the final data-frame and store it as a _csv_ file and perform some basic analytics about the unavailability of some data.  

#### Websites used  
---  
* I have first used [this]("https://en.wikipedia.org/wiki/List_of_Indian_film_actors") and [this]("https://en.wikipedia.org/wiki/List_of_Indian_film_actresses") **Wikipedia** pages, which give the complete list of actors(first link) and actresses(second link).  

* These pages provide links to the specific pages of the respective actor/actress. Which are stored and then each one is visited to extract the information.  

* From each page I have taken the person's name, his description, _i.e._ the first paragraph in the page, and check for the availability of his image. If present it is downloaded, else a **Google** search is made with his name as query and an image is downloaded from the results.  

* Since age in Wikipedia is present in different places in different formats, and due to the unavailability of height of most of the actors. I have used separate Google searches to get these information.

#### Final output  
---  
* There are a total of **1732** Indian movie celebrities.  

* The description is also cleaned to remove new line characters and wiki-links, and some heights are stored in sentences.  

* The entire data-frame is stored as a csv file in _data.csv_.  

* The data-frame contains a column storing the image file name, and all those files are stored in the _Images_ folder.  

* Age information of _102_ celebrities, height information of _186_ celebrities and description of _2_ celebrities is unavailable.   
