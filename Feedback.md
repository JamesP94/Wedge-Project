## Feedback 

For what it's worth, I think you handled this project in a smart way. You have a number of classmates who have decided that the data cleaning hill is one they will die on. That's fine 
for people who are doing every exercise and really learning the underlying Python, but it's very hard to LLM one's way to that solution, as we're all learning. 

One high-level point: all of your committed notebooks have runtime errors in them or places where you've stopped execution. For assignments, just run everything through so I
can see that it worked. Outside of classes, just clear all output and the do the save and commit. 

I'm going to read your files in order and give you feedback
as I move through them, from Task 1 to Task 3. 


### Task 1

#### Cleaning

* If you're defining the schema, I wouldn't do almost everything as an object. Although this is in the ELT paradigm (since those objects are typically string-like).
* Your replace line is putting in "null", but that will go in as a string in GBQ. This is probably the place you could have asked for some help. I think if you had mapped all of your null values to "" then you might have solved your problems.

#### Uploading

* Here you have sensible column values in the schema. You'd want to have the pandas column types matched to the schema column types.
* Smart to use the load-table-from-file. Most people did a pandas `read_csv` followed by some pandas-gbq, but your approach is more efficient in terms of both memory and code. 

### Task 2

Nice job on this task, everything looks good. Except for your commentary about it in the submission. Here's what you wrote: 

> This file takes a sample of 500 rows from the wedge transactions dataset and saves it to a csv file called 'query_results.csv'

When I read this, my heart sank, because I was afraid I'd have to ask you to re-do this. As it turns out, you _didn't_ do what you wrote. Instead, you selected 500 _card numbers_. Then you 
selected _every_ row for those card numbers. It's weird to me that you wrote something this factually inaccurate on your submission. 

### Task 3

* Nice job on this, very efficient. ChatGPT slipped in a print error on you when it called the DB Postgres instead of SQLite. Other than that it all looks good. 
