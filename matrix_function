import numpy as np

def calculate(list):
  #check if the list contains 9 numbers by transforming list into 3x3 matrix
  try:
    a = np.reshape(list, (3,3))
  #set error message when list doesn't contain 9 numbers
  except:
    raise ValueError("List must contain nine numbers.")
  else:
    #calculate values along axis1, axis2 and flattened matrix and change them into lists for inclusion in dictionary
    means = [(np.mean(a, axis=0).tolist()), (np.mean(a, axis=1).tolist()), (np.mean(a))]
    variances = [(np.var(a, axis=0).tolist()), (np.var(a, axis=1).tolist()), (np.var(a))]
    stddevs = [(np.std(a, axis=0).tolist()), (np.std(a, axis=1).tolist()), (np.std(a))]
    maxv = [(np.max(a, axis=0).tolist()), (np.max(a, axis=1).tolist()), (np.max(a))]
    minv = [(np.min(a, axis=0).tolist()), (np.min(a, axis=1).tolist()), (np.min(a))]
    sums = [(np.sum(a, axis=0).tolist()), (np.sum(a, axis=1).tolist()), (np.sum(a))]
    #create dictionary
    calculations = dict([('mean', means), ('variance', variances), ('standard deviation', stddevs), ('max', maxv), ('min', minv), ('sum', sums)])

    return calculations
