# -
将 1, 2, \ldots , 91,2,…,9 共 99 个数分成 33 组，分别组成 33 个三位数，且使这 33 个三位数构成 1 : 2 : 31:2:3 的比例，试求出所有满足条件的 33 个三位数。

for i in range(123,333):
    j = str(i*2)
    k = str(i*3)
    i = str(i)
    a = {i[0],i[1],i[2],j[0],j[1],j[2],k[0],k[1],k[2]}
    if len(a)==9 and ("0" not in a):
      print(int(i), int(j), int(k))
