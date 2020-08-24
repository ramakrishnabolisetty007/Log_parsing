# Log_parsing
>Parsing of log files using pandas

Requirements : Python 3.7.9, Pandas 1.0.4

Dependencies : pprint, pprint, IPython

## Setup
- Download Python 3.7.9 from this [link]( https://www.python.org/downloads/).
- Follow this [guide](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html) to install pandas.
- Follow this [guide](https://jupyter.org/install) to install Jupyter notebook.
- Download my notebook from [here](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Submission.ipynb) and leverage it's features or even better [clone this repository](https://github.com/ramakrishnabollisetty007/Log_parsing.git).


## Implementation

- Sample log file data in raw format has been used for analysis.
- Standard format of the log : dd24-024.compuserve.com - - [03/Aug/1995:18:30:07 -0400] "GET /cgi-bin/imagemap/countdown69?187,293 HTTP/1.0" 302 110
- Converted plain file into CSV using regex.
- Used random buckets of 65,000 line items are used to test the utility. 

## Features

- Top 10 most requested resources
- Percentage of Successful and Unsuccessful requests
- Top 10 Unsuccessful requests
- Top 10 hosts interacting with the system
- Top 10 hosts with their top page hits
- Percentile of requests
- Median value for the Response size (in bytes)

## Merits of the current version

- Single I/O operation.
- No primitive looping techniques(for,while etc.) used.
- Handles edge cases in user inputs through command line interface.



## Tests
![User options](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Options%20for%20users.PNG)

### Sample Input 
![Sample Input](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Sample%20input.PNG)
![Top 10 most requested resources](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Top%2010%20accessed%20resources.PNG)
![Percentage of Successful and Unsuccessful requests](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Percentage%20of%20successful%20and%20unsuccessful%20requests.PNG)
![Top 10 Unsuccessful requests](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Top%2010%20Unsuccessful%20requests.PNG)
![Top 10 hosts interacting with the system](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Top%2010%20hosts%20interacting%20with%20the%20system.PNG)
![Top 10 hosts with their top page hits](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Top%2010%20hosts%20with%20their%20top%20page%20hits.PNG)
![Normalised percentages of requests](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Normalised%20percentages%20of%20requests.PNG)
![Median value for the Response size](https://github.com/ramakrishnabollisetty007/Log_parsing/blob/master/Tests/Median%20value%20for%20the%20Response%20size%20(in%20bytes).PNG)


## Scope for improvements

- Instead of top 10 items, it can be top n items based on user input.
- User to enter the path to read the file from.
- To make this utility a configuration based utility (No code utility).
- Visualisations such as graphs,scatter plots can be added to declutter the statistics.
- Since there is no circular reference of memory, Garbage collection can be diabled to improve memory consumption for cases where we are dealing with huge data.



