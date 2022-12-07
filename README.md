# Web-scraping-of-NIH-and-ASCO-for-retrieval-of-cancer-research-centers-and-oncologist-data
Using web scraping and Biopython to extract cancer data from NIH and ASCO to build a consolidated program for search and retrieval of Cancer Research centers and oncologists


### Motivation
Cancer research is crucial to improve the prevention, detection and treatment of these cancers, and ensure that survivors live longer, better quality lives. Research also helps identify the causes of cancer and is pointing the way to improved methods of diagnosis and treatment. On these lines, statistical tools in Data analysis and biostatistics help us find avenues to understand trends in cancer technology , novel findings and reliability of research that can help make diagnosis more accessible and the process smoother altogether.
Packages/Libraries used :
* Pandas
* Numpy
* Biopython - specifically the Entrez database
* BeautifulSoup
 
Introduction
In this assignment, Web Scraping has been done on Multiple research websites under the NIH so as to form a consolidated consortium to access data relating to oncologists, medical practitioners and cancer research centres. The data pertaining to the National Cancer Institute (NCI) afilliated research centres has been downloaded and converted to a CSV file from the website : https://www.cancer.gov/research/nci-role/cancer-centers. 


We then proceed to scrape data from the Cancer.Net portal’s  The ‘Find an Oncologist Database’ is made available by ASCO as an informational resource for patients and caregivers. The database includes the names of physicians and other health professionals from certain ASCO membership categories who have given their permission to be identified publicly. We match the oncologists obtained from the ASCO portal to the hospitals from the NCI portal in the last step ( we add the names of additional hospitals not present in the previous list and save both the data in the onco_df frame.
We then move on to using the Biopython’s entrez functionality that helps us access the Pubmed database. From this we obtain the Pubmed ID of the corresponding authors in the onto_df data frame. This gives us useful information about the research works carried out by the oncologist on the specialization of cancer or any novel method they have been working on.
![image](https://user-images.githubusercontent.com/68393451/206109396-83bea83a-b2ba-402b-bff7-4d328f87afac.png)


EDA is then performed on the consolidated data frame to understand the correlation between number of oncologists and performance of the cancer institute (We cross check if our Data Analysis matches with the trends shown in the news).
We further move on the explore the number of publications amongst the Oncologist’s community and rank the researchers as well as plot the distribution.

![image](https://user-images.githubusercontent.com/68393451/206109153-429c5046-7852-4e73-8db6-13a125e0322b.png)



