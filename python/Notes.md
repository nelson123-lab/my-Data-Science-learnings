## List Comprehension

- To get all the values of a list except a specific value.
suits = ["h","c", "d", "s"]
noclubs = [x for x in suits if x != "c"]

## General Notes

To upgrade pip
  python -m pip install --upgrade pip    
  
- Sort dictionaries according with the keys
  dict(sorted(res.items()))

To sort dictonaries according to the values
p = sorted(record.items(),key=lambda x: x[1])
print(p)


