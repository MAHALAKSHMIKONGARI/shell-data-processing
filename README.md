# shell data processing

The curl commands used are,
- ```curl "https://en.wikipedia.org/wiki/Area_51"```
- ```curl "https://en.wikipedia.org/wiki/Area_51" -O data.txt```

Bash commands used to sort the data are:
- ```tr ' ' '\12' < data.txt```
- ```tr ' ' '\12' < data.txt | sort```
- ```tr ' ' '\12' < data.txt | sort | uniq -c```
- ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr```

To Redirect the output to result.txt:
- ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt```

## Important data:
- The -n flag is used to sort the values based on numeric data.
- The -r flag is used to sort the values in the reverse order.
- In a single letter flag, only one dash is used.
- We have to use 2 dashes for the flag with more than one letter.


