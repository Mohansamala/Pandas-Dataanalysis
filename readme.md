
# National Achievement Survey Analysis


## Datasets

The National Achievement test was taken by 185348 students in 6,722 schools across 33 states and union territories of India. 
Data collected not only involves marks but also different aspects of students  involving family background, daily routine and poverty.
3 datasets are provided      
 1.nas pupil marks       
 2.nas columns     
 3.nas labels      
## steps in analysis of data

### required python dependancies
import pandas as pd    
import numpy as numpy           
import matplotlib as mpl           
import matplotlib.cm as cm          
import matplotlib.pyplot as plt     

### 1.Loading  of data and counting no of null values 
Maths %                   92661 out of 185348           
Reading %                 92073           
Science %                 94342      
Social %                  95765        
### 2.finding and deleting duplicates
Nas pupil data contains 16 duplicate rows these are to be deleted 
 

### 3.handling nans
Presence of above 90000 nans in three columns can affect data analysis .if all nans are removed then analysis will be losing 90000 rows which will impact data analysis                             
Filling of nans using mean will be a better                         

# Questions               

## How do boys and girls perform across states?                                

   Performance of student is calucated by the average of marks in subjects MATHS,SCIENCE,SOCIAL,READING ,AFTER filling the nan values in these columns using mean method(fillna) .                           
   After analysing the data ,   following are deduced                                        
          1.IN 12 states Boys perform better than girls            
          2.In 21 states Girls  perform better than boys                    
          3.     state records in best(max) performance of boys                
          4.    state records in best(ma)   performance of girls                  
          5.     state accounts for maxdifference between girls and boys with      
          6.     state accounts for mindifference between girls   and boys with      
          7.      state accounts for poor performance of boys and     state for girls       
Code snippet can be 
    

### Graph
![alt text](performance.png "perfoormance of boys and girls")

By plot  and analysis  we can state that  girls perform better than Boys  overall.
## Does southindian excel at math and science ?
creating a dataframe which contains maths and science marks

marks["MSc"]=marks["Maths %"]+marks["Science %"] #perecentage of marks in maths and science MSc        

and plotting based on two states south and rest of india          
### plot
![alt text](mSc.png "southindians(blue) vs rest indians performance in maths and science")           


## No ,

### Thankyou
