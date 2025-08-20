Log 05-20-2025
I am having a mathematical error in my .fit function where I am getting NaN or Not a Number. I need to look deeper in the model training process to see what has failed.


Googled possibilities:
This is the first place you should always check. Garbage in, garbage out.

1 - NaN values already in the dataset: If you feed the model data that already contains NaNs, its calculations will produce NaNs.

2 - Zeros or very large numbers: Operations like division by zero or taking log(0) will result in NaN or infinity, which quickly corrupts all subsequent calculations.

3 - Poorly scaled features: If you have features with vastly different scales (e.g., one feature from 0-1 and another from 1,000-100,000), it can make the math unstable.

Log 05-20-2025
Added In initial ranking step 3 to create new columng "fit_score."
Need to verify human biasness to see if this can intelligently understand similar words to pull out other candidates.
