# Case_Study2

## Data Scraping
In this case study we have learned how to scrape data **legally** from sports website using **Python** language.

The process of scraping relies on using for loops to automate the process. We used the **request** library and the **get** function to get a response object (to grap the code of a page) and assign it to a variable 'page' as shown here: 

page = requests.get('https://www.premierleague.com/clubs')

Then, we get the content of the response object using function **.content** provided by **request** library **('page.content')**. The document of this content is obtained using the **'fromstring'** function provided by **'html'** package of the **lxml** model the result is stored in a variable 'tree' as shown here: 
tree = html.fromstring(page.content). Finally, using the cssselect method provided by HTML to locate and select elements and their childern from the 'tree' element we have gotten in the previous step.

After getting our data, we did some preprocessing to clean and get the data ready for analysis.

