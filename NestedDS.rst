.. code:: ipython3

    set1 = {1,2,3,4,5}
    set2 = {5,6,7,8,9,10}
    print(set1.intersection_update(set2))  # set1 mein sirf wo numbers chhorta hai jo set2 mein bhi hon. updated list k bd kuch common nhi tbhi none
    print(set1.difference_update(set2)) #same element hoga tou usko remove krdegi aur baaki ki list improve krdega
    print(set1.symmetric_difference(set2)) #ascending order wise diplay krdega
    print(set1.symmetric_difference_update(set2)) #Kyunki set1 ab khali set hai, tou set 2 kay saray elements set1 main chale tbhi none aya


.. parsed-literal::

    None
    None
    {5, 6, 7, 8, 9, 10}
    None
    

#NESTED DATA STRUCTURED

.. code:: ipython3

    #NESTED LISTS:
    names = ["ayesha","zainab","abeeha","khalil",[8,9,10,11,12,13], #1d
    [1,2,3,4,5,6,7], #2d
    ("hello","brother","sister"),{"a","b","c","d"}] #2d
    print(len(names))
    print(len(names[4]))
    print("one",names[4]) 
    print("two",names[4][4])
    print("three",names[5][2])
    print("four",names[4][5])
    print(type(names[6]))
    print(type(names[7]))
    #set main indexing nhi hoti is liye wo nhi add hoskta tbhi 7th main indexing nhi ho rhi thi
    


.. parsed-literal::

    8
    6
    one [8, 9, 10, 11, 12, 13]
    two 12
    three 3
    four 13
    <class 'tuple'>
    <class 'set'>
    

.. code:: ipython3

    table = [
        [1,2,3,["ned","iba"]],
        [4,5,6,["a","b"],7],
        [7,8,9] ] #this whole list is 3 dimension list
    print(len(table)) #agar 2 sets of braacket maximum lg rhe tou wo hmesha 2d list hai
    print(table[2][0]) #[row][coloumn]
    print(table[1][3])
    print(table[1][3][0]) #1list ka 3 element and uska 0 element
    print("total length",len(table))
    


.. parsed-literal::

    3
    7
    ['a', 'b']
    a
    total length 3
    

.. code:: ipython3

    table1 = [
        [1,2,3,["ned","iba"]],
        [4,5,6,["a","b"],7],
        [7,8,9],{"uni_name": "fuuast","total_student":"50","dept": "cs"}]
    print(len(table1))
    print(table1[3])
    print(table1[3]["dept"])
    


.. parsed-literal::

    4
    {'uni_name': 'fuuast', 'total_student': '50', 'dept': 'cs'}
    cs
    

#nested dictionary


.. code:: ipython3

    uni_students = {
        "names":["ayesha","zainab","abeeha","khalil"],
        "ages":[20,22,23,25],
        "degree":["bs","be","phd","ma"],
        "intitute":["fast","fuuast","ned","ku"],
        "subjects":{"ayesha":["computer","eng"],
                    "zainab":["ur","sci"],
                    "abeeha":["ai","ds"]}
                    
                    
    }
    print(len(uni_students))
    print(uni_students["ages"][2])
    print(uni_students["subjects"]["ayesha"][1])


.. parsed-literal::

    5
    23
    eng
    

