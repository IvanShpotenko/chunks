# chunks
Generator that yields successive n-sized chunks from an iterable.     
Each yilded chunk is a generator of size n.     
That means you have to empty (iterate over) current chunk in order to get the right result.     
Last chunk will be sized as is and will not be padded with any value.       

```python
for chunk in chunks(range(25), n=7):
    print(list(chunk))
```

```
>>> [0, 1, 2, 3, 4, 5, 6]
>>> [7, 8, 9, 10, 11, 12, 13]
>>> [14, 15, 16, 17, 18, 19, 20]
>>> [21, 22, 23, 24]
```
