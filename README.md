# tweets-language
#The dataset contains Twitter data and you will iterate over entries in a column to build a dictionary in which the keys are the name of #languages and the values are the number of tweets in the given language, then return the resulting dictionary from within the function.
#the file tweets.csv is available.
import pandas as pd
df=pd.read_csv('tweets.csv')
def count_entries(df,col_name='lang')
    """Return a dictionary with counts of occurrence as value for each key."""
    #initialize an empty dictionary: langs_count
    langs_count={}
    #extract column from DataFrame:col
    col=df[col_name]
    for entry in col:
        if entry in langs_count.keys():
            langs_count[entry]+=1
        else:
            langs_count[entry]=1
     return lang_count   
#call count_entries():result
result=count_entries(tweets_df)
print(result)

import pandas as pd
df=pd.read_csv('tweets.csv')
def count_entries(df,*args)
    """Return a dictionary with counts of occurrence as value for each key."""
    #initialize an empty dictionary: langs_count
    langs_count={}
    try:
        for entry in args:
            if entry in langs_count.keys():
                langs_count[entry]+=1
            else:
                langs_count[entry]=1
         return lang_count   
     except:
         print('The DataCampt does not have a ' + entry +' column.')
#call count_entries():result
result=count_entries(tweets_df,'lang','source')
print(result)

        
      
        



