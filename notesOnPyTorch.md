### Storage, tensor, offset and stride

Page 22-29. A storage is a contiguous 1D array. Values are stored in storages. A tensors accesses a storage using `offset`, indices, and `stride`. 

Page 29. `contiguous()` converts a non-contiguous tensor to a contiguous one. I expect a new storage to be created, but I found that the resulting storage has the same id as the old one, which means they are the same storage. I don't understand how laying out two storages gives you different results. See [notebook](question_contiguous.ipynb). 