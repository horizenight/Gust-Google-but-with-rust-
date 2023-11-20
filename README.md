# Gust-Google-but-with-rust-


### Implementing search engine for docs.gl so that we can search inside function rather than only names for better usability. 


## Google in Rust => 
Gust : Tf-idf => term frequency inverse document frequency
value = how frequent it is in that document / how freuqent it is in other document
It tells us it is noise or not 

## Problem statement => 
```docs.gl``` cam only search through names but not the things that are inside the the document

1. Convert XML into text 
2. Text into buffer 


## Search Idea =>
 Take prompt from user and tokenize it then each token is used to compute the tf-idf for each document 
we sum them up and we get ranking for each individual document
then we sort and give top 10 
