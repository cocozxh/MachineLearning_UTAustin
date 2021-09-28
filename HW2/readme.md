# Independent Components Analysis (ICA)
Separate different independent signals from several mixed signals
## Dataset
Three or two signals selected from given five signals with length 44000
## Procedure
![image](https://user-images.githubusercontent.com/49115822/135134354-439d400c-57dc-4aa6-9557-09dc01496265.png)
## Parameter
**A** is a NXN matrix (N is the number of signals selected to be mixed), its element are randomly initialized under a uniform distribution between 0 to 1.  
Elements of **W** are random initialized under a uniform distribution between 0 to 0.000001.  
**Learning rate** is 0.0001.  
**100000 iterations** each experiment
## Result and Improvements
Since the order of recovered signal is unknown, we cannot figure out which original signal a particular recovered signal is corresponded with, 
I chose to flip the recovered signal matrix, compute all the possibility of correspondence and chose the biggest correlation as result.  
The best correlation achieved by separating ths signals mixed from three original ones is 0.92066527.  
The best correlation achieved by separating ths signals mixed from two original ones is 0.99806129.
