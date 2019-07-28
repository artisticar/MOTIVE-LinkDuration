# MOTIVE_LinkDuration

Please make sure that **NumPy** and **Pandas** are installed. 

<br>

There're several important variables that you may want to control before executing the program.

Instructions are attached below. 

After making the changes the way you want, simply run through all the cells in the designated order and you'll get an output csv file, with the last column denoting contact duration.

<br>

**The 11th line in the 7th cell**

```python
# 	The number below denotes the number of rows we want to extract the 
# contact duration from the NGSIM.csv file. 
# 	In this case, we're extracting contact duration from the first 2000 rows.
# 	You can customize the number of rows you want to process by changing the number.
# 	To process the whole file, delete these two lines from the code.
if i > 2000:  
        break
```

<br>

**The 26th line in the 7th cell**

```python
# 	The number below denotes the communication range.
#		In this case it's set to 50 meters. 
if relative_distance <= 50:  
				......
    		......
```

<br>

**The last line in the 8th cell**

```python
# 	You can modify the first argument to change the name of the output csv file
what_we_want = np.savetxt("output.csv", output_array, delimiter=",",fmt = "%s")
```

<br>

### **About the dataset**

The NGSIM.csv file in this repository contains only the first 5000 rows of the original csv file. To process the whole dataset(approximately 12 million rows), please

- download it from the website of [U.S. Department of Transportation](https://catalog.data.gov/dataset/next-generation-simulation-ngsim-vehicle-trajectories)
- rename it as NGSIM.csv 
- replace the NGSIM.csv file in the repository