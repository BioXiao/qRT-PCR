# qPCR 

### Process You qRT-PCR Results Results Easy  
====


     
This python script aims at calculating the **Delta_Ct, Delta_Delta_Ct and FoldChange** value which
produced by Quantitative real time polymerase chain reaction.
    
**Pandas**, a python data analysis tool, is required for using this script. I use Ipython notebook as my interpreter.
    
The following file formats are supported: **xls, xlsx, csv, txt. 
    
In addition, your should specify **reference control** name and **expriment control** name for your own data sets.
    
For ABi 7900 users, data column names must be 'Sample Name','Detector Name','Ct','Ct Mean'. But 'Ct StdEV' is optional.

For ABi ViiA 7 users, you can use readExecl.py to extract data computing results directly.

##Useage

Python2.7 or Python3

e.g. python readExecl.py -f foo.xls --header 35 --tail 5 -r GAPDH -c hESC -o 20150625

##To Do

1. process data automatically without pre-filter outliner mannully.
2. Generate Plots using Matplotlib automatically 
3. Generate Matplotlib Plotting Scripts for customized modification

