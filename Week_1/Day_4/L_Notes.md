# Lecture Notes Week 1 Day 4

API request calls are always unordered

## Good modules for formatting JSON strucutres:

- ### For jupyter notebooks
    - from IPython.display import JSON
    - JSON(our_JSON_strucutre)

- ### Standard Python Library
    - import json
    - our_JSON_strucuture.json()

JSON structures only allow dictionaries and lists

 ## enumerate() is a convenient way to loop through a list:

 enumerate(iterable, start=0)

- for i, elem in enumerate(our_list):
    - print(i) ---> 0, 1, 2
    - print(elem) ---> elements in our_list

