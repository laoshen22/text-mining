

Text Data Presentation
========================================================
width: 1000
height: 800
author: Lisa Ling
date: December 09 2015
transition: rotate


<small> 
Department of Statistics   
Dalhousie University   
</small>


Outline
========================================================


- What text data looks like
- Goal--Structured data
- Questions--Information Extraction


What text data looks like
========================================================
The radiology data will contribute to improving accuracy of our hierarchical tree structure model. However, this is an unstructured text data.

![alt text](data_pic.png)



Goal--What we are interested in
========================================================

We're only interested in specific kinds of information in text, the relation between radiology test findings and their status, i.e. **“which finding in which status”**.

 Finding   | status  
 ----------|--------------------
 mass      | no/yes         
 ascites   | small/malignent/no         
 collection| no/yes        


Goal--Structured Data
========================================================

![alt text](goal.png)


Goal
========================================================

1. Build a system that extracts structured data from unstructured text
2. Robust methods for identifying the entities and relationships described
in a text. Reduce error and misunderstand.
3. Model evaluation


Question--Information Extraction
========================================================
type: section

- Fetch the key words (abnormal, metastatic, collection, mass etc.) 
- Spelling Correction


Question--Information Extraction
========================================================
transition: none
incremental: true

### Fetch the key words 



- Consider synonyms for key words
    - metastatic, metastases, metastasis
- Consider various expressions. 
    - No significant abnormality
    - No acute intracranial abnormality
    - No due to cervicalspine abnormality
    - is uncertain whether this is a true lesion
 



Question--Information Extraction 
========================================================
transition: none
incremental: true


- Consider positive/negtive
    - No acute intracranial abnormality/ No abnormality
    - abnormality
- Consider categorical levels
    - no signs of ascites
    - very small amount of ascites
    - malignant ascites   
    
    

Question--Information Extraction 
========================================================
transition: none
incremental: true

### Spelling Correction


- **Spelling mistake**: abnormaliti
- **No space**: noevidence, nohemorrhage, noabnormality, theright, nodefinite, metastaticdisease
- **dash sign**: intra abdominal, intra-abdominal
  



Example 1
========================================================




Example 2 
========================================================




Example 2--What we did  
========================================================


```
[[1]]
 [1] " is mild dependent atelectasis"                
 [2] " no pleural or pericardial effusion"           
 [3] " is diffuse colonicdiverticulosis"             
 [4] "normal"                                        
 [5] " consistent with acute diverticulitis"         
 [6] " is noevidence of perforation or focal abscess"
 [7] " is noascites"                                 
 [8] " no aggressive appearing osseous lesion"       
 [9] " is acute sigmoid diverticulitis"              
[10] " without associatedabscess or perforation"     
[11] " uncomplicated diverticula"                    
```


We'd love to listen to your suggestion! Thank you!
========================================================




<img src="datacloud.png" style="background-color:transparent; border:0px; box-shadow:none;" height="500px" width="700px"></img>


