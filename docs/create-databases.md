
In this section, you will learn how to create the databases files on your local computer. Use the following code for creating the databases. 

```python
import msdb
```

```python
msdb.create_db()
```

It will display some ipywdigets inside which you can enter the info (db name and folder path) required to create the databases files (see figure below).


![Alt text](images/create_db.png){: .img-Large align=left }
/// caption
Ipywidgets to be filled when creating the databases files
///

Once you have filled the ipywidgets with valid info, clicking on the button 'Create databases' will lead to the creation of the [databases files](https://g-patin.github.io/msdb/databases-files/) in the registered folder. Additionally, it will register the database in the [*db_config.json*](https://g-patin.github.io/msdb/db_config/) file. 


