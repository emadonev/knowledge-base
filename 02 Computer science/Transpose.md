TAGS: #python #programming #array #data 

When we have an array dataset, we can use `.T` to transpose the given matrix or `DataFrame`. 
1. Our data is ordered so that it has columns of data:
```python
data[id] = [ [time1, mag1, magErr1], 
				 [time2, mag2, magErr2], 
				 [time3, mag3, magErr3] ]
```
and so on. 
2. Using `.T` the array would be transposed, like so:
```python
data[id].T = [ [time1, time2, time3], 
			   [mag1, mag2, mag3], 
			   [magErr1, magErr2, magErr3] ]
```
- all of the data is now nicely ordered into rows depending on the type: all the time data in one row, all the magnitude data in one row and all of the errors in one row.
3. Now, we can assign variables to this, like so:
```python
time = [time1, time2, time3] 
mag = [mag1, mag2, mag3] 
magErr = [magErr1, magErr2, magErr3]
```
And we have a nicely sorted and ordered (in this case time series) data!

