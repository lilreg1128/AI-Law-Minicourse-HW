# AI-Law-Minicourse-HW
## Supreme Court Topic Modeling
### Step 1: Data Collection and Preparation
Grab the data from the website using BeautifulSoup within your defined function Beautiful_soup_grabber. Year_getter runs through the years and grabs the relevant documents then converts resutls to a data frame. It then defines the column names, checks values and serializes the data into a byte stream.
### Step 2: Data Collection and Preparation
Collects descriptions of the cases and other details from the cases and creates a table and then saves.
### Step 3: Data Processing
Scrub the data to purge state names, case names, common stop words, names, dates, numbers, etc. This allows the program to process the appropriate data, i.e. the content of the cases. 
### Step 4: Topic Modeling Method Testing
Running the different topic modeling algorithms: Latent Dirchlet Allocation (LDA) model, the Latent Semantic Analysis (LSA) model, and the Non-negative Matrix Factorization (NMF) model. 
### Step 5: Topic Modeling Application to Data
Description of NMF.
## TensorFlow Tutorial
### Step 1: Download the data
In this step the code is assigning the web page to the variable 'url,' defining the function 'maybe_download' and then making a call to the function with the name of the file to be used and the expected size of the file. This downloads the file and returns the download but also checks for an error if the the file isn't found. The function 'read_data' is also defined which is then caled with the file returned from 'maybe_download.' This function parses the data into a list of words.
### Step 2: Build dictionary/rare words->UNK token
The vocabulary size is assigned, the function 'build_dataset' is defined and run with the list of words and the size defined. The function takes the list of words, counts each word that appears and creates an array which maps the words with a code. It also  reversed the ap to create a reversed_dictionary, i.e. the words are mapped to their keys and then the keys are also mapped to the words. The function is run and the returned results are put into four global variables. It then deletes the variable 'vocabulary' which was the downloaded file in the original format.
### Step 3: Generate training batch
The 'generate_batch' function is defined which creates the training batch from the global variable data based on the inputs defined as batch size, number of skips, and skip window for the skip-gram model. The batch is a subset of the data.
### Step 4: Build and Train
### Step 5: Begin Training
