# esi-copy-ara-sarqi-qo-hamar
eduardi komic mi poqr nver sax gisher mernelov ashxtelem
n = int(input("input number!!!!"))
n1 = 0
v = 0

#e=n % 10
d = n // 1 % 10
c = n // 10 % 10
b = n // 100 % 10
a = n // 1000
n = str(n)

result = ""
for i in n:
    max = -1
    for j in n:
        if not(j in result) and int(j) > max:
            max = int(j)
    if max != -1:
        result += str(max)
print(result)
#16842-vor false lini
if a/b == b/c and b/c == c/d:
    print("True")
else:
    f = int(input("input another num!!! "))
    print(f)
    e = f % 10
    w = f // 10 % 10
    s = f // 100 % 10
    l = f // 1000 % 10
    q = f // 10000
    while f != 0:
        v += 1
        f = f//10
    print("count of num: " + str(v))
    if v == b+c:
        print("True")
    else:
        print("false")
        f = [q, l, s, w, e]
        sort = sorted(f, reverse=True)
        print(sort[0])
    if q == e:
        print("yes")
    elif q+l+s+w+e > 20:
        print("edit with code 1 ")
    else:
        print("invalid code!!!")
    g = int(input("input num for division: "))
    sum = 0
    multy = 1
    for i in f:
        if i / g == 0:
            sum += i
        elif i / 2 != 0 and i / 3 != 0:
            multy *= i
    print("The sum of nums: " + str(sum) + "\n" + "The multiply of nums: " + str(multy))
    count = 0
    for j in str(f):
        j = int(j)
        count += 1
        sum += j
        multy *= j
    print("The sum of nums: " + str(sum) + "\n" + "The multiply of nums: " + str(multy) + "\n" + "count of num: " + str(count))
    s2 = "2"
    f1 = f
    if s2 in str(f):
        f = int(f)
        while f != 0:
            q1 = f % 10
            print(q1)
            f = f // 10
        f1 = str(f1)
        a = len(f1)
        b = 10 ** (a - 1)
        f1 = int(f1)
        while b >= 1:
            c = f1 // b % 10
            print(c)
            b = b // 10
    sum1 = 0
    sum2 = 0
    index = 0
    for i in str(f1):
        print(index, i)
        index += 1
        if index % 2 == 0:
            sum1 += int(i)
        else:
            sum2 += int(i)
    print(sum1 == sum2)
