---
cover: ../.gitbook/assets/_1fcc2772-08ad-454f-bf7b-a5d67147f489.jpg
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🐍 Open CSV file in Python

### Reading

Use reader() to create an object for reading data from a CSV file. The reader  can be used as an iterator to process the rows of the file in order.

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

The first argument to **reader()** is **the source of text lines**. In this case, it is a file, but any iterable is accepted (stringIO instances, lists, etc.). Other optional arguments can be given to control how the input data is parsed.

### Writing

Writing CSV files is just as easy as reading them. Use writer() to create an object for writing, then iterate over the rows, using writerow() to print them.

```python
import csv
import sys

f = open(sys.argv[1], 'wt')
try:
    writer = csv.writer(f)
    writer.writerow( ('Title 1', 'Title 2', 'Title 3') )
    for i in range(10):
        writer.writerow( (i+1, chr(ord('a') + i), '08/%02d/07' % (i+1)) )
finally:
    f.close()

print open(sys.argv[1], 'rt').read()
```
