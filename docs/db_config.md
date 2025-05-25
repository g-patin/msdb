
## 1. **Description**

The *db_config* file is a json file inside which basic information related to the databases are being stored. Currently, only the name and location of the databases are being stored inside the json file. This file enables the `msdb` package to find the location of the databases files so that basic operations (create, read, update, delete)  on the files can be performed. 


The json file is located inside the folder of the `msdb` package. To know where it is on your local computer, import the `msdb` package inside a jupyter notebook and simply run the name of the package, as illustrated below. It will return the location of the *\__init__.py* file. The *db_config* file is in the same folder as the  *\__init__.py* file.

```python
import msdb
```

```python
msdb
```

<div class="output-area">
<pre>
< module 'msdb' from '/home/john/anaconda3/lib/python3.11/site-packages/msdb/__init__.py'>
</pre>
</div>


## 2. **Read content**

To read the content of the *db_config* file, use the following lines of code:

```python
import msdb
```

```python
# display the content of the db_config.json file
# we can see that I created two databases : 'db' and 'MFT'
msdb.get_config_file()
```

<div class="output-area">
<pre>
{'databases': {'db': {'path_folder': '/home/john/Documents/databases'},    
  'MFT': {'path_folder': '/home/john/Documents/MFT/databases'}}}
</pre>
</div>

&nbsp;

For more information on how to manage the content of the *db_config* file, consult the [Manage the db_config file](https://g-patin.github.io/msdb/manage_db_config/) section.
