# AkNishida
#pythonスキルチェック_B008_地下アイドルの夢_20190107
#https://paiza.jp/works/python3/primer/beginner-python2/4012

import sys

array = []
for line in sys.stdin.readlines():
    array.append(line.rstrip().split(' '))
#print(array)
menmber_N=(array[0][0])
event_M=(array[0][1])
#print(menmber_N)
#print(event_M)
array_r=array[1:]
#print(array_r)

each_event=[]
for i in array_r:
    #print(i)
    #print(sum(int(p) for p in i))
    sum_i = sum(int(p) for p in i)
    if sum_i >  0:
        each_event.append(sum_i)
    else:
        pass
    #for k in i:
        #print(k)
        #each_event.append(k)
#print(each_event)
print(sum(int(q) for q in each_event))

