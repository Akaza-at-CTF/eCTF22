# I can do this all day

> Tony Stark: a hacker who's faster than ultron? he could be anywhere GLOBAL. And as this is the center of everything, I'm just a REGULAR guy looking for a needle in the world's biggest haystack.
> 
> World Hub Tech: How do you find it? <with puzzled EXPRESSION>
> 
> Tony Stark: pretty simple. you bring a magnet.
> 
> Flag format: CTF{...}

The goal is to search through all the files to find the flag using a command such as grep (the hint is the capitalised words). We can also join the files together and use `ctrl+F`.
  
```python
import pathlib

f = open("all.txt", "w")

for file in pathlib.Path("./icandothisallday").iterdir():
    r = open(file, "r")
    for line in r:
        f.write(line)
    r.close()

f.close()
```
  
The flag is `CTF{d3cry471ng_nu3l34r_c0d35}`
