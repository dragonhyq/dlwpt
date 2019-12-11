### Chapter 2

Page 22-29. A storage is a contiguous 1D array. Values are stored in storages. A tensors accesses a storage using `offset`, indices, and `stride`. 

Page 29. `contiguous()` converts a non-contiguous tensor to a contiguous one. I expect a new storage to be created, but I found that the resulting storage has the same id as the old one. but `data_ptr()` returns different values. I do not know what happens to the storage when `contiguous()` is called. See [notebook](question_contiguous.ipynb). 

Page 37. PyTorch uses a trailing underscore to indicate that a function operates in-placeon a tensor (such as `Tensor.sqrt_`).