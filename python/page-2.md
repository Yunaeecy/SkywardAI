---
cover: ../.gitbook/assets/_1fcc2772-08ad-454f-bf7b-a5d67147f489.jpg
coverY: 0
---

# 🐍 Open CSV file in Python

### Reading

Use rader() to create an object for reading data from a CSV  file. The reader  can be used as an iterator to process the rows of the file in order.

```python
import csv
import sys

f = open(sys.argv[1], 'rt')
try:
    reader = csv.reader(f)
    for wor in reader:
        print row
finally:
    f.close()thon
```
