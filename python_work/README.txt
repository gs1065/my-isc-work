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








>>> import numpy as np
>>> x = range(1, 11)
>>> a1 = np.array(x, np.int32)
>>> a2 = np.array(x, np.float32)
>>> print a1.dtype
int32
>>> print a2.dtype
float32
>>> arr = np.zeros((2, 3, 4))
>>> arr = np.ones((2, 3, 4))
>>> arr = np.arange(1000)
>>> a = np.array([2, 3.2, 5.5, -6.4, -2.2, 2.4])
>>> a[1]
3.2000000000000002
>>> a[1:4]
array([ 3.2,  5.5, -6.4])
>>> print arr
[  0   1   2   3   4   5   6   7   8   9  10  11  12  13  14  15  16  17
  18  19  20  21  22  23  24  25  26  27  28  29  30  31  32  33  34  35
  36  37  38  39  40  41  42  43  44  45  46  47  48  49  50  51  52  53
  54  55  56  57  58  59  60  61  62  63  64  65  66  67  68  69  70  71
  72  73  74  75  76  77  78  79  80  81  82  83  84  85  86  87  88  89
  90  91  92  93  94  95  96  97  98  99 100 101 102 103 104 105 106 107
 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125
 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143
 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161
 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179
 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197
 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215
 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233
 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251
 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 267 268 269
 270 271 272 273 274 275 276 277 278 279 280 281 282 283 284 285 286 287
 288 289 290 291 292 293 294 295 296 297 298 299 300 301 302 303 304 305
 306 307 308 309 310 311 312 313 314 315 316 317 318 319 320 321 322 323
 324 325 326 327 328 329 330 331 332 333 334 335 336 337 338 339 340 341
 342 343 344 345 346 347 348 349 350 351 352 353 354 355 356 357 358 359
 360 361 362 363 364 365 366 367 368 369 370 371 372 373 374 375 376 377
 378 379 380 381 382 383 384 385 386 387 388 389 390 391 392 393 394 395
 396 397 398 399 400 401 402 403 404 405 406 407 408 409 410 411 412 413
 414 415 416 417 418 419 420 421 422 423 424 425 426 427 428 429 430 431
 432 433 434 435 436 437 438 439 440 441 442 443 444 445 446 447 448 449
 450 451 452 453 454 455 456 457 458 459 460 461 462 463 464 465 466 467
 468 469 470 471 472 473 474 475 476 477 478 479 480 481 482 483 484 485
 486 487 488 489 490 491 492 493 494 495 496 497 498 499 500 501 502 503
 504 505 506 507 508 509 510 511 512 513 514 515 516 517 518 519 520 521
 522 523 524 525 526 527 528 529 530 531 532 533 534 535 536 537 538 539
 540 541 542 543 544 545 546 547 548 549 550 551 552 553 554 555 556 557
 558 559 560 561 562 563 564 565 566 567 568 569 570 571 572 573 574 575
 576 577 578 579 580 581 582 583 584 585 586 587 588 589 590 591 592 593
 594 595 596 597 598 599 600 601 602 603 604 605 606 607 608 609 610 611
 612 613 614 615 616 617 618 619 620 621 622 623 624 625 626 627 628 629
 630 631 632 633 634 635 636 637 638 639 640 641 642 643 644 645 646 647
 648 649 650 651 652 653 654 655 656 657 658 659 660 661 662 663 664 665
 666 667 668 669 670 671 672 673 674 675 676 677 678 679 680 681 682 683
 684 685 686 687 688 689 690 691 692 693 694 695 696 697 698 699 700 701
 702 703 704 705 706 707 708 709 710 711 712 713 714 715 716 717 718 719
 720 721 722 723 724 725 726 727 728 729 730 731 732 733 734 735 736 737
 738 739 740 741 742 743 744 745 746 747 748 749 750 751 752 753 754 755
 756 757 758 759 760 761 762 763 764 765 766 767 768 769 770 771 772 773
 774 775 776 777 778 779 780 781 782 783 784 785 786 787 788 789 790 791
 792 793 794 795 796 797 798 799 800 801 802 803 804 805 806 807 808 809
 810 811 812 813 814 815 816 817 818 819 820 821 822 823 824 825 826 827
 828 829 830 831 832 833 834 835 836 837 838 839 840 841 842 843 844 845
 846 847 848 849 850 851 852 853 854 855 856 857 858 859 860 861 862 863
 864 865 866 867 868 869 870 871 872 873 874 875 876 877 878 879 880 881
 882 883 884 885 886 887 888 889 890 891 892 893 894 895 896 897 898 899
 900 901 902 903 904 905 906 907 908 909 910 911 912 913 914 915 916 917
 918 919 920 921 922 923 924 925 926 927 928 929 930 931 932 933 934 935
 936 937 938 939 940 941 942 943 944 945 946 947 948 949 950 951 952 953
 954 955 956 957 958 959 960 961 962 963 964 965 966 967 968 969 970 971
 972 973 974 975 976 977 978 979 980 981 982 983 984 985 986 987 988 989
 990 991 992 993 994 995 996 997 998 999]
>>> a = np.array([[2, 3.2, 5.5, -6.4, -2.2, 2.4], [1, 22, 4, 0.1, 5.3, -9], [3, 1, 2.1, 21, 1.1, -2]])
>>> print a
[[  2.    3.2   5.5  -6.4  -2.2   2.4]
 [  1.   22.    4.    0.1   5.3  -9. ]
 [  3.    1.    2.1  21.    1.1  -2. ]]
>>> a[:, 3]
array([ -6.4,   0.1,  21. ])
>>> array[1:4, 0:4]
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'array' is not defined
>>> a[1:4, 0:4]
array([[  1. ,  22. ,   4. ,   0.1],
       [  3. ,   1. ,   2.1,  21. ]])
>>> a[1:, 2]
array([ 4. ,  2.1])
>>> a[0, :]
array([ 2. ,  3.2,  5.5, -6.4, -2.2,  2.4])
>>> a[1:4, 0:3]
array([[  1. ,  22. ,   4. ],
       [  3. ,   1. ,   2.1]])
>>> a[1:3, 0:4]
array([[  1. ,  22. ,   4. ,   0.1],
       [  3. ,   1. ,   2.1,  21. ]])
>>> a[1:, 0:4]
array([[  1. ,  22. ,   4. ,   0.1],
       [  3. ,   1. ,   2.1,  21. ]])
>>> a[0, :]
array([ 2. ,  3.2,  5.5, -6.4, -2.2,  2.4])
>>> a[1, :]
array([  1. ,  22. ,   4. ,   0.1,   5.3,  -9. ])
>>> a[2, :]
array([  3. ,   1. ,   2.1,  21. ,   1.1,  -2. ])
>>> a[0:1, 1:4]
array([[ 3.2,  5.5, -6.4]])
>>> import numpy as np
>>> arr = np.array([range(4), range(10, 14])
  File "<stdin>", line 1
    arr = np.array([range(4), range(10, 14])
                                          ^
SyntaxError: invalid syntax
>>> arr = np.array([range(4), range(10, 14)]
... 
... 
... print arr.shape
  File "<stdin>", line 4
    print arr.shape
        ^
SyntaxError: invalid syntax
>>> print arr.shape
(1000,)
>>> 
KeyboardInterrupt
>>> import numpy as np
>>> arr = np.array([range(4), range(10, 14)]
... print arr.shape
  File "<stdin>", line 2
    print arr.shape
        ^
SyntaxError: invalid syntax
>>> print arr.shape
(1000,)
>>> print arr.size
1000
>>> print arr.max
<built-in method max of numpy.ndarray object at 0x1200120>
>>> print arr.max(_
... print arr.max(_
  File "<stdin>", line 2
    print arr.max(_
        ^
SyntaxError: invalid syntax
>>> print arr.max()
999
>>> print arr.min()
0
>>> arr = np.array([range(4), range(10, 14)]
... 
... 
... 
...  
... 
... print arr
  File "<stdin>", line 7
    print arr
        ^
SyntaxError: invalid syntax
>>> print arr.shape
(1000,)
>>> arr = np.array([range(4), range(10, 14)]
... 
... print ar.shape
  File "<stdin>", line 3
    print ar.shape
        ^
SyntaxError: invalid syntax
>>> print arr.shape
(1000,)
>>> arr = np.array([range(4), range(10, 14)])
>>> print arr.shape
(2, 4)
>>> print arr.max()
13
>>> print arr.min()
0
>>> print np.reshape(arr, (2, 2, 2))
[[[ 0  1]
  [ 2  3]]

 [[10 11]
  [12 13]]]
>>> print np.transpose(arr)
[[ 0 10]
 [ 1 11]
 [ 2 12]
 [ 3 13]]
>>> print np.ravel(arr)
[ 0  1  2  3 10 11 12 13]
>>> print arr.astype(np.float64)
[[  0.   1.   2.   3.]
 [ 10.  11.  12.  13.]]
>>> 




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


masked arrays
>>> import numpy.ma as MA#
>>> import numpy.ma as MA
>>> marr = MA.masked_array(range(10), fill_value = -999)
>>> print marr, marr.fill_value
[0 1 2 3 4 5 6 7 8 9] -999
>>> marr[2] = MA. masked
>>> print marr
[0 1 -- 3 4 5 6 7 8 9]
>>> print marr.mask
[False False  True False False False False False False False]
>>> narr = MA.masked_where(marr > 6, marr)
>>> print narr
[0 1 -- 3 4 5 6 -- -- --]
>>> x = MA.filled(narr)
>>> print x
[   0    1 -999    3    4    5    6 -999 -999 -999]
>>> print type(x)
<type 'numpy.ndarray'>
>>> m1 = MA.masked_array(1,9))
  File "<stdin>", line 1
    m1 = MA.masked_array(1,9))
                             ^
SyntaxError: invalid syntax
>>> m1 = MA.masked_array(range(1, 9))
>>> print m1
[1 2 3 4 5 6 7 8]
>>> print m2
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'm2' is not defined
>>> m2 = m1.reshape(2, 4)
>>> print m2
[[1 2 3 4]
 [5 6 7 8]]
>>> m3 = MA.masked_greater(m2, 6)
>>> print m3
[[1 2 3 4]
 [5 6 -- --]]
>>> res = m3 - np.ones((2, 4))
>>> print res
[[0.0 1.0 2.0 3.0]
 [4.0 5.0 -- --]]
>>> print type(res)
<class 'numpy.ma.core.MaskedArray'>
>>> y = m3 * 100
>>> print y
[[100 200 300 400]
 [500 600 -- --]]
>>> 
