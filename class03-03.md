## Reading Notes: Class 03

### Readings: FileIO & Exceptions

#### Reading and Writing Files in Python (Guide)

One of the common tasks in coding is reading and writing files. According to Mertz (n.d.), "a file is a contiguous set of bytes used to store data"; this file can be a text file or an executable program.

Three main parts of modern file system (Mertz, n.d.):

- Header
- Data
- EOF or End of file

The header is a metadata about file contents, the data contains file or information written by the creator, while end of file is a " special character that indicates the end of the file" (Mertz, n.d.).

**File Path**

The file path is required to access the file:

- Folder path - folder's location in the system/device
- File name - the name of the file
- Extension - "the end of the file path pre-pended with a period (.) used to indicate the file type" (Mertz, n.d.).

**Opening and closing a file in Python**

To open a file:

```
open("sample.text") or
file = open("sample.text")

```

To close the file:

```
An example provided by Mertz (n.d.) in his article:

reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
    

```


References:

Mertz, J. (n.d.). *Reading and writing files in python (Guide)*. Real Python. https://realpython.com/read-write-files-python/
