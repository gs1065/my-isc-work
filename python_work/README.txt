python work

To do a git push

#exit python

>>> exit()

#get in directory you want to push file from

[user01@unst26 ~]$ cd my-isc-work/python_work

#do a git add

[user01@unst26 python_work]$ git add README.txt

#do a git commit and name file, then input password

[user01@unst26 python_work]$ git commit -m"pythonstuff"
[master f80274b] pythonstuff
 1 files changed, 159 insertions(+), 0 deletions(-)
[user01@unst26 python_work]$ git push
Counting objects: 7, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 1.46 KiB, done.
Total 4 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://gs1065@github.com/gs1065/my-isc-work.git
   c72140e..f80274b  master -> master


Day 4
#list starts square brackets, tuple starts normal brackets. Tuple imutable sequance (can't change), list can change. Can convert a list to a tuple. i.e. tup = tuple(a) where a is list a. Tuples handy as can assign variables, i.e. x, y, z = a 
# then data files

Dictionaries
[user01@unst26 ~]$ python 2.7
python: can't open file '2.7': [Errno 2] No such file or directory
[user01@unst26 ~]$ cd my-python-worl
bash: cd: my-python-worl: No such file or directory
[user01@unst26 ~]$ python2.7
Python 2.7.3 (default, Feb 21 2014, 13:11:38) 
[GCC 4.4.7 20120313 (Red Hat 4.4.7-3)] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> a = set([0, 1, 2, 3, 4, 5])
>>> b = set([2, 4, 6, 8])
>>> print a.union(b)
set([0, 1, 2, 3, 4, 5, 6, 8])
>>> print a.intersection(b)
set([2, 4])
>>> band = ["mel", "geri", "victoria", "mel", "emma"]
>>> mkdir counts
  File "<stdin>", line 1
    mkdir counts
               ^
SyntaxError: invalid syntax
>>> mkdir "counts"
  File "<stdin>", line 1
    mkdir "counts"
                 ^
SyntaxError: invalid syntax
>>> counts = {}
>>> for name in band: 
...     if name not in counts:
...         counts[name] = 1
...     else
  File "<stdin>", line 4
    else
       ^
SyntaxError: invalid syntax
>>>     else:
  File "<stdin>", line 1
    else:
    ^
IndentationError: unexpected indent
>>>     else:
  File "<stdin>", line 1
    else:
    ^
IndentationError: unexpected indent
>>> 
KeyboardInterrupt
>>> band = ["mel", "geri", "victoria", "mel", "emma"]
>>>     if name not in counts:
  File "<stdin>", line 1
    if name not in counts:
    ^
IndentationError: unexpected indent
>>>     if name not in counts:
KeyboardInterrupt
>>> band = ["mel", "geri", "victoria", "mel", "emma"]
>>> counts = {}
>>> for name in band:
...     if name not in counts:
...         counts[name] = 1
...     else:
...         counts[name] = += 1
  File "<stdin>", line 5
    counts[name] = += 1
                    ^
SyntaxError: invalid syntax
>>> 
KeyboardInterrupt
>>> python2.7
  File "<stdin>", line 1
    python2.7
            ^
SyntaxError: invalid syntax
>>> 
KeyboardInterrupt
>>> band = ["mel", "geri", "victoria", "mel", "emma"]
>>> counts = {}
>>> 
>>> 
>>> for name in band:
...     if name not in counts:
...         counts[name] = 1
...     else:
...         counts[name] += 1
... 
>>> for name in counts: 
...     print name, counts[name]
... 
mel 2
geri 1
emma 1
victoria 1
>>>         counts[name] += 2
  File "<stdin>", line 1
    counts[name] += 2
    ^
IndentationError: unexpected indent
>>> band = ["mel", "geri", "victoria", "mel", "emma"]
>>> counts = {}
>>> for name in band:
...     if name not in counts:
...         counts[name] = 1
...     else:
...         counts[name] += 2
... 
>>> for name in counts: 
...     print name, counts[name]
... 
mel 3
geri 1
emma 1
victoria 1
>>>     print name, counts[name]
  File "<stdin>", line 1
    print name, counts[name]
    ^
IndentationError: unexpected indent
>>> if {}: print 'hi' # is not True
... 
>>> d = {"maggie": "uk", "ronnie": "usa"}
>>> dir(d)
['__class__', '__cmp__', '__contains__', '__delattr__', '__delitem__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__gt__', '__hash__', '__init__', '__iter__', '__le__', '__len__', '__lt__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__setitem__', '__sizeof__', '__str__', '__subclasshook__', 'clear', 'copy', 'fromkeys', 'get', 'has_key', 'items', 'iteritems', 'iterkeys', 'itervalues', 'keys', 'pop', 'popitem', 'setdefault', 'update', 'values', 'viewitems', 'viewkeys', 'viewvalues']
>>> ['__class__', ..., 'viewvalues']
  File "<stdin>", line 1
    ['__class__', ..., 'viewvalues']
                  ^
SyntaxError: invalid syntax
>>> ['__class__', ..., 'viewvalues']
  File "<stdin>", line 1
    ['__class__', ..., 'viewvalues']
                  ^
SyntaxError: invalid syntax
>>> print d.items()
[('maggie', 'uk'), ('ronnie', 'usa')]
>>> print d.keys()
['maggie', 'ronnie']
>>> print d.values()
['uk', 'usa']
>>> d.get("maggie", "nowhere")
'uk'
>>> d.get("ringo", "nowhere")
'nowhere'
>>> res = d.setdefault("mikhail", "ussr")
>>> print res, d"mikhail"]
  File "<stdin>", line 1
    print res, d"mikhail"]
                        ^
SyntaxError: invalid syntax
>>> print res, d["mikhail"]
ussr ussr
>>> res = d.setdefault("rob", "cars")
>>> print res,  d["rob"]
cars cars

