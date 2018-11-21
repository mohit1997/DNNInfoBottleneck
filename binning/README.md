# Code for Different Kind of binning

How to change binning while computing Mutual Information

In `MNIST_ComputeMI.py` or `IBnet_ComputeMI.py`, change the following line,

```python
binxm, binym = simplebinmi.bin_calc_information2(saved_labelixs, activity, binsize)  # for constant bin size
This binsize is replaced by

# sz = (np.max(activity)-np.min(activity))/10.0      for min-max approach
# or
# sz = np.std(activity)*1.0                          for standard deviation approach

```


