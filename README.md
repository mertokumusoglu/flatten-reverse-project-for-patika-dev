# flatten-reverse-project-for-patika-dev

#flatten list sorusu

list1 = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
flatten_list = []

def flattened(l):
    for newlist in l:
        if type(newlist) == list:
            flattened(newlist)
        else:
            flatten_list.append(newlist)
    return flatten_list
            
print(flattened(list1))


----------------------------------------------------------------------------------

#reverse list sorusu

list2 = [[1, 2], [3, 4], [5, 6, 7]]

def reversened(l):
    l.reverse()
    for newlist in l:
        if type(newlist) == list:
            reversened(newlist)
print(list2)
print(reversened(list2))
print(list2)
