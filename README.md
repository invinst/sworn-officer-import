
The import requires our current django CPDB to run, but the logic should
be understandable to anyone with python experience.

For the officers_import_data.csv the first column is either:

- a positive integer, then it is matched as an officer

- a -1: this means we will create the officer, the following rows are
 that officers new ID

- a 0: could not be matched because there are multiple records this
 could belong to. Should be decided manually. I've added the possible
 matching/conflicting officer IDS after the last star column, starting
 at column U

a -2: possible merge, same as with 0, the possible merging officer ids are listed at the end
