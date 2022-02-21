# PC2.0-Automation

### Find_duplicates.py
  
Find the duplicates of the Item-IDs, Item-Names
  and price-entity-ids in the Negative-Flow-sheet.xlsx. 
  
**IMPORTANT** :  In order to run the code you need the following files
  in a directory :
  > - Find_duplicates.py
  > - setup_env.sh

Your folder structure should look like this :  
```commandline
PC2.0-Automation
|
├── Find_duplicates.py
├── <Negative-flow-sheet>.xlsx
└── setup_env.sh
```

**NOTE**: You need an Excel workbook (mentioned above as `<Negative-flow-sheet>.xlsx`) as the input and the desired outputs will be available in the folder `Output`. 
The filename `<Negative-flow-sheet>.xlsx` means you need to put your Excel workbook here. 
 
To parse the Excel file you need to follow the below steps exactly :

**Step-1** : Run the shell script, from the terminal, to install dependencies.
```setup-environment 
 ./setup_env.sh
```
**NOTE :** After this step please verify if a folder has been created in your current 
directory with the name `pc2Automation`. This is the virtual environment where all dependencies are 
installed.

After step 1 your folder structure should look like this :
```commandline
PC2.0-Automation
|
├── Find_duplicates.py
├── setup_env.sh
├── <Negative-flow-sheet>.xlsx
└── pc2Automation
```


**Step-2** : Activate the Python virtual environment by executing the following
command from your current directory 

```activate-environment
 source ./pc2Automation/bin/activate
```
You should now see the following in your terminal :
```commandline
(pc2Automation) cb-it-00-0000@CB-IT-00-0000s-MacBook-Pro PC2.0-Automation %
```

**Step-3** : If your Step-2 is complete then all you have to do is run the following :
```commandline
(pc2Automation) cb-it-00-0000@CB-IT-00-0000s-MacBook-Pro PC2.0-Automation % python3 Find_duplicates.py --filename <Negative-flow-sheet>.xlsx 
```
If this executes then you will see the following lines:
```commandline
(pc2Automation) cb-it-01-1487@CB-IT-01-1487s-MacBook-Pro PC2.0-Automation % python3 Find_duplicates.py --filename <Negative-flow-sheet>.xlsx 
Processing file : <Negative-flow-sheet>.xlsx
File has been processed. :)
```
also, you will have a new folder in your current directory.
```commandline
PC2.0-Automation
|
├── Find_duplicates.py
├── setup_env.sh
├── <Negative-flow-sheet>.xlsx
├── Output
└── pc2Automation
```

#### NOTE : `New PC2.0 - Negative flow sheet.xlsx` is an example input xlsx file. You can follow the format for the file headers. The `Output` folder contains sample outputs from that input file.

