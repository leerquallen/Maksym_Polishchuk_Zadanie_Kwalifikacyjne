Task 1:

The structure of the quantity.csv file initially presented some challenges as the columns were not named. To address this, I made certain assumptions based on my familiarity with the data.csv and prices.csv files. I assumed that the first column represented 'part_number' and the second column represented 'quantity.'

However, it's important to note that 'part_number' values were often repeated across multiple rows, and this raised questions about how to properly interpret the data. To handle this ambiguity, I made the assumption that different rows with identical 'part_number' values represented different sources of the same part. In other words, the individual parts were generally the same, but they were sourced from different suppliers or locations.

For the first solution, I chose to aggregate the quantities by combining rows with identical 'part_number' values. I summed up the 'quantity' values, and in cases where the count exceeded 10, I replaced the value with '>10'. This approach was based on the assumption that we wanted to consolidate the data while keeping the total quantity within a reasonable range.

However, given the uncertainty about the correct interpretation, I also created an alternative solution. In the second solution, I did not aggregate quantities and simply merged all rows, ignoring duplicate 'part_number' values. This approach provides an unaltered view of the data with no consolidation.

To facilitate the review and comparison of these two solutions, I have provided code files, CSV results, and text comparisons, each named with "aggregate_quantities" and "no_aggregate_quantities" attachments, respectively.

Task 2:

I compared the content of CSV files using Pandas and pandasql. Results were exported in Excel and CSV formats for compatibility, and SQL queries were saved in text file for reference.

Task 3:

Task 3 proved to be unexpectedly challenging, primarily due to the unconventional structure of the "PP0006_MULTI.txt" file. The main challenges arose from the inconsistent formatting of the data, which made it difficult to convert the file into a CSV format or use a row-splitting approach for data structuring. The lack of consistent separators between records further complicated the task.

I also explored pattern matching as a potential solution, but the complex data structure required equally intricate patterns. Additionally, the large file size added to the complexity of the process, making this approach less practical.

While I considered using external software like Apache Spark, the task instructions specifically required the use of Pandas for solving both Tasks 1 and 3. As a result, I was unable to employ alternative tools to tackle the challenges presented by Task 3.

Regrettably, I must conclude that I was unable to successfully solve Task 3 within the given constraints. If the opportunity arose to consult with the person who provided the task, I would gladly take that chance to seek guidance and attempt to resolve the task with additional insights and an extended timeframe.
