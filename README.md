# Case_Study2

## Data Scraping
In this case study we have learned how to scrape data **legally** from sports website using **Python** language.

The process of scraping relies on using for loops to automate the process. We used the **request** library and the **get** function to get a response object (to grap the code of a page) and assign it to a variable 'page' as shown here:

page = requests.get('https://www.premierleague.com/clubs')

Then, we get the content of the response object using function **.content** provided by **request** library **('page.content')**. The document of this content is obtained using the **'fromstring'** function provided by **'html'** package of the **lxml** model the result is stored in a variable 'tree' as shown here: 
tree = html.fromstring(page.content). Finally, using the cssselect method provided by HTML to locate and select elements and their childern from the 'tree' element we have gotten in the previous step. After collecting our data, we did some preprocessing to clean and get the data ready for analysis, highlighted which types are related to this case study, and some hypothesis testing was conducted at the end..

During the work on this case study, members conducted several meetings on teams through all phases of work. 
Ideas were shared by all members before perfoming the work on Jupyter Notebook. After agreeing on ideas and the work flow, each task was assigned to a specific member to divide the work load.

The assigned tasks were as follows:

**Mohammed Atros**: performed data scraping, feature generation and some preprocessing

**Ala'a Abu Qtaish**: Performed additional preprocessing and highlited differences in the data through multiple visualizings 
and illustrations

**Anbara Al-Jamal**: Highlited the types of experiments used through the project

**Anoud Khazaa'lah**: Formalated a hypothesis and tested it using unpaired t-test   

