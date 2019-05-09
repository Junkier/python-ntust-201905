

```python
f = open("sample.csv",mode="r",encoding="utf8")
data = f.readlines()
f.close()
```


```python
print(data)
```

    ['貨品分類,中文貨名,英文貨名,國家,數量,數量單位,重量,重量單位,價值\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",巴林,0,-   ,8000,KGM ,411\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",日本,0,-   ,10800,KGM ,696\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",加拿大,0,-   ,108631,KGM ,7365\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",沙烏地阿拉伯,0,-   ,503000,KGM ,24919\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",其他大洋洲國家,0,-   ,11695,KGM ,729\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",阿拉伯聯合大公國,0,-   ,29000,KGM ,1274\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",科威特,0,-   ,121536,KGM ,6128\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",美國,0,-   ,749982,KGM ,46022\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",香港,0,-   ,72,KGM ,2\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",澳大利亞,0,-   ,69570,KGM ,4786\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",關島,0,-   ,8618,KGM ,458\n', '12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",加拿大,0,-   ,0,TNE ,43\n', '12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",美國,0,-   ,0,TNE ,9\n', '12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",菲律賓,0,-   ,0,TNE ,6\n', '52114200005,牛仔布, Denim,中國大陸,11398,MTK ,1991,KGM ,902\n', '52114200005,牛仔布, Denim,日本,14364,MTK ,3898,KGM ,1596\n', '52114200005,牛仔布, Denim,印尼,21998,MTK ,3869,KGM ,1543\n', '52114200005,牛仔布, Denim,印度,7212,MTK ,2185,KGM ,513\n', '52114200005,牛仔布, Denim,柬埔寨,28081,MTK ,9915,KGM ,2469\n', '52114200005,牛仔布, Denim,馬來西亞,8925,MTK ,3598,KGM ,575\n', '52114200005,牛仔布, Denim,越南,139191,MTK ,53225,KGM ,12330\n', '52114200005,牛仔布, Denim,賴索托,6894,MTK ,2771,KGM ,435\n']
    


```python
# print(data)

# for line in data:
#     print(line.strip())
    
   
# for line in data:
#     categoryNo = line.split(",")[0]
#     name = line.split(",")[1]
#     print(categoryNo,name)


for line in data:
    print(line.strip())
    print("Country : ",line.split(",")[4])

```

    貨品分類,中文貨名,英文貨名,國家,數量,數量單位,重量,重量單位,價值
    Country :  數量
    3032300007,冷凍吳郭魚," Tilapias, frozen",巴林,0,-   ,8000,KGM ,411
    Country :  巴林
    3032300007,冷凍吳郭魚," Tilapias, frozen",日本,0,-   ,10800,KGM ,696
    Country :  日本
    3032300007,冷凍吳郭魚," Tilapias, frozen",加拿大,0,-   ,108631,KGM ,7365
    Country :  加拿大
    3032300007,冷凍吳郭魚," Tilapias, frozen",沙烏地阿拉伯,0,-   ,503000,KGM ,24919
    Country :  沙烏地阿拉伯
    3032300007,冷凍吳郭魚," Tilapias, frozen",其他大洋洲國家,0,-   ,11695,KGM ,729
    Country :  其他大洋洲國家
    3032300007,冷凍吳郭魚," Tilapias, frozen",阿拉伯聯合大公國,0,-   ,29000,KGM ,1274
    Country :  阿拉伯聯合大公國
    3032300007,冷凍吳郭魚," Tilapias, frozen",科威特,0,-   ,121536,KGM ,6128
    Country :  科威特
    3032300007,冷凍吳郭魚," Tilapias, frozen",美國,0,-   ,749982,KGM ,46022
    Country :  美國
    3032300007,冷凍吳郭魚," Tilapias, frozen",香港,0,-   ,72,KGM ,2
    Country :  香港
    3032300007,冷凍吳郭魚," Tilapias, frozen",澳大利亞,0,-   ,69570,KGM ,4786
    Country :  澳大利亞
    3032300007,冷凍吳郭魚," Tilapias, frozen",關島,0,-   ,8618,KGM ,458
    Country :  關島
    12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",加拿大,0,-   ,0,TNE ,43
    Country :  加拿大
    12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",美國,0,-   ,0,TNE ,9
    Country :  美國
    12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",菲律賓,0,-   ,0,TNE ,6
    Country :  菲律賓
    52114200005,牛仔布, Denim,中國大陸,11398,MTK ,1991,KGM ,902
    Country :  11398
    52114200005,牛仔布, Denim,日本,14364,MTK ,3898,KGM ,1596
    Country :  14364
    52114200005,牛仔布, Denim,印尼,21998,MTK ,3869,KGM ,1543
    Country :  21998
    52114200005,牛仔布, Denim,印度,7212,MTK ,2185,KGM ,513
    Country :  7212
    52114200005,牛仔布, Denim,柬埔寨,28081,MTK ,9915,KGM ,2469
    Country :  28081
    52114200005,牛仔布, Denim,馬來西亞,8925,MTK ,3598,KGM ,575
    Country :  8925
    52114200005,牛仔布, Denim,越南,139191,MTK ,53225,KGM ,12330
    Country :  139191
    52114200005,牛仔布, Denim,賴索托,6894,MTK ,2771,KGM ,435
    Country :  6894
    


```python
# Read

f = open("sample.csv",mode="r",encoding="utf8")
# data = f.readlines()


# data = f.read(197)

# print(data)
# print(type(data))

data = f.readline()
data += f.readline()
data += f.readline()
data += f.readline()

print(data)

```

    貨品分類,中文貨名,英文貨名,國家,數量,數量單位,重量,重量單位,價值
    3032300007,冷凍吳郭魚," Tilapias, frozen",巴林,0,-   ,8000,KGM ,411
    3032300007,冷凍吳郭魚," Tilapias, frozen",日本,0,-   ,10800,KGM ,696
    3032300007,冷凍吳郭魚," Tilapias, frozen",加拿大,0,-   ,108631,KGM ,7365
    
    


```python
# Write
words = [
    "frozen",
    "This is an apple",
    "test write file",
    "今天禮拜一",
    "明天會放假"
]


# f2 = open("test1.txt",mode="w")

# # \n :換行字元


# f2.write("Hello world!")
# f2.write("\n")

# f2.write("Python test.")
# f2.write("\n")

# f2.write("~~~~~~")
# f2.write("\n")

# f2.close()

f2 = open("test1.txt",mode="w")

for w in words :
    f2.write(w)
    f2.write("\n")

f2.close()
```


```python
# Append
words = [
    "Avengers",
    "每天都在下雨",
    "Py~~~~~~thon",
    "Anaconda",
    "原萃綠茶"
]

f3 = open("test2.txt",mode="a")

for w in words:
    f3.write(w)
    f3.write("\n")
    
f3.close()
```


```python
# with open("test3.txt",mode="w") as f4:
#     for w in words:
#         f4.write(w)
#         f4.write("\n")
    # ....
    
    
    
with open("sample.csv",mode="r",encoding="utf8") as f5:
    data2 = f5.readlines()
    
print("Done!")    
    
print("-"*50)
print(data2)
```

    Done!
    --------------------------------------------------
    ['貨品分類,中文貨名,英文貨名,國家,數量,數量單位,重量,重量單位,價值\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",巴林,0,-   ,8000,KGM ,411\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",日本,0,-   ,10800,KGM ,696\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",加拿大,0,-   ,108631,KGM ,7365\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",沙烏地阿拉伯,0,-   ,503000,KGM ,24919\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",其他大洋洲國家,0,-   ,11695,KGM ,729\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",阿拉伯聯合大公國,0,-   ,29000,KGM ,1274\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",科威特,0,-   ,121536,KGM ,6128\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",美國,0,-   ,749982,KGM ,46022\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",香港,0,-   ,72,KGM ,2\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",澳大利亞,0,-   ,69570,KGM ,4786\n', '3032300007,冷凍吳郭魚," Tilapias, frozen",關島,0,-   ,8618,KGM ,458\n', '12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",加拿大,0,-   ,0,TNE ,43\n', '12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",美國,0,-   ,0,TNE ,9\n', '12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",菲律賓,0,-   ,0,TNE ,6\n', '52114200005,牛仔布, Denim,中國大陸,11398,MTK ,1991,KGM ,902\n', '52114200005,牛仔布, Denim,日本,14364,MTK ,3898,KGM ,1596\n', '52114200005,牛仔布, Denim,印尼,21998,MTK ,3869,KGM ,1543\n', '52114200005,牛仔布, Denim,印度,7212,MTK ,2185,KGM ,513\n', '52114200005,牛仔布, Denim,柬埔寨,28081,MTK ,9915,KGM ,2469\n', '52114200005,牛仔布, Denim,馬來西亞,8925,MTK ,3598,KGM ,575\n', '52114200005,牛仔布, Denim,越南,139191,MTK ,53225,KGM ,12330\n', '52114200005,牛仔布, Denim,賴索托,6894,MTK ,2771,KGM ,435\n']
    


```python
# Encoding
words = [
    "Avengers",
    "每天都在下雨",
    "Py~~~~~~thon",
    "Anaconda",
    "原萃綠茶"
]

f3 = open("testA.txt",mode="w",encoding="utf8")

for w in words:
    f3.write(w)
    f3.write("\n")
    
f3.close()
```


```python
# words = [
#     "Avengers",
#     "每天都在下雨",
#     "Py~~~~~~thon",
#     "Anaconda",
#     "原萃綠茶"
# ]

# f3 = open("testA.txt",mode="w",encoding="utf8")

# for w in words:
#     f3.write(w)
#     f3.write("\n")
    
# f3.close()


# words = [
#     "可口可樂",
#     "星巴克",
#     "Python好難學阿",
#     "練習練習",
#     "放棄放棄"
# ]

# f3 = open("testB.txt",mode="w",encoding="utf8")

# for w in words:
#     f3.write(w)
#     f3.write("\n")
    
# f3.close()


# words = [
#     "Notepad++",
#     "禮拜四總愛下雨",
#     "放假放假",
#     "禮拜六放假",
#     "Lemon Tea ~~~"
# ]

# f3 = open("testC.txt",mode="w",encoding="utf8")

# for w in words:
#     f3.write(w)
#     f3.write("\n")
    
# f3.close()
```


```python
def readData(fileName):
#     f6 = open("testC.txt","r",encoding="utf8")    
    f6 = open(fileName,"r",encoding="utf8")
    dataC = f6.readlines()

    z=1
    for w in dataC :
        print("Line : " , z , " , " , "Message : ", w.strip())
        z+=1
    


# f4 = open("testA.txt","r",encoding="utf8")
# dataA = f4.readlines()

# i=1
# for w in dataA :
#     print("Line _ " , i , " , " , "Message _ ", w.strip())
#     i+=1

# print("-"*50)
    
# f5 = open("testB.txt","r",encoding="utf8")
# dataB = f5.readlines()

# j=1
# for w in dataB :
#     print("Line _ " , j , " , " , "Message _ ", w.strip())
#     j+=1
    
    
# print("-"*50)
    
# f6 = open("testC.txt","r",encoding="utf8")
# dataC = f6.readlines()

# z=1
# for w in dataC :
#     print("Line : " , z , " , " , "Message : ", w.strip())
#     z+=1


###########################################################################

readData("testA.txt")

print("-"*50)

readData("testB.txt")

print("-"*50)

readData("testC.txt")

```

    Line :  1  ,  Message :  Avengers
    Line :  2  ,  Message :  每天都在下雨
    Line :  3  ,  Message :  Py~~~~~~thon
    Line :  4  ,  Message :  Anaconda
    Line :  5  ,  Message :  原萃綠茶
    --------------------------------------------------
    Line :  1  ,  Message :  可口可樂
    Line :  2  ,  Message :  星巴克
    Line :  3  ,  Message :  Python好難學阿
    Line :  4  ,  Message :  練習練習
    Line :  5  ,  Message :  放棄放棄
    --------------------------------------------------
    Line :  1  ,  Message :  Notepad++
    Line :  2  ,  Message :  禮拜四總愛下雨
    Line :  3  ,  Message :  放假放假
    Line :  4  ,  Message :  禮拜六放假
    Line :  5  ,  Message :  Lemon Tea ~~~
    


```python
# def  test_func(name , age , remark=“good”):
#     print(name)
#     print(“Age : {}”.format(age))
#     print(”Remark is {}”.format(remark))
#     return “done”


# test_func(“Jeff”,18)

def sayMyName(name , age , remark="ABC", A=1 ,B=2):
    print("Name : " , name)
    print("Age : "  , age)
    print("Remark : ",remark)
    

sayMyName("Jeff",20)

print("-"*50)

sayMyName("Leo",25)

print("-"*50)

sayMyName("test",40)
```

    Name :  Jeff
    Age :  20
    Remark :  ABC
    --------------------------------------------------
    Name :  Leo
    Age :  25
    Remark :  ABC
    --------------------------------------------------
    Name :  test
    Age :  40
    Remark :  ABC
    


```python
def add(a,b):
    return a+b

def add2(a,b,c):
    k = a+b+c
    print("In function : " , k)
    return k


result = add(2,8)
print(result)


result2 = add2(1,7,9)
print(result2)

print("Out of function : ",k)
```

    10
    In function :  17
    17
    


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-11-8ead966cae86> in <module>
         15 print(result2)
         16 
    ---> 17 print("Out of function : ",k)
    

    NameError: name 'k' is not defined



```python
with open("sample.csv","r",encoding="utf-8") as inFile:
    _data = inFile.readlines()
# print(_data)

for w in _data:
    print(w.strip())
    value = w.split(",")[-1]
```

    貨品分類,中文貨名,英文貨名,國家,數量,數量單位,重量,重量單位,價值
    3032300007,冷凍吳郭魚," Tilapias, frozen",巴林,0,-   ,8000,KGM ,411
    3032300007,冷凍吳郭魚," Tilapias, frozen",日本,0,-   ,10800,KGM ,696
    3032300007,冷凍吳郭魚," Tilapias, frozen",加拿大,0,-   ,108631,KGM ,7365
    3032300007,冷凍吳郭魚," Tilapias, frozen",沙烏地阿拉伯,0,-   ,503000,KGM ,24919
    3032300007,冷凍吳郭魚," Tilapias, frozen",其他大洋洲國家,0,-   ,11695,KGM ,729
    3032300007,冷凍吳郭魚," Tilapias, frozen",阿拉伯聯合大公國,0,-   ,29000,KGM ,1274
    3032300007,冷凍吳郭魚," Tilapias, frozen",科威特,0,-   ,121536,KGM ,6128
    3032300007,冷凍吳郭魚," Tilapias, frozen",美國,0,-   ,749982,KGM ,46022
    3032300007,冷凍吳郭魚," Tilapias, frozen",香港,0,-   ,72,KGM ,2
    3032300007,冷凍吳郭魚," Tilapias, frozen",澳大利亞,0,-   ,69570,KGM ,4786
    3032300007,冷凍吳郭魚," Tilapias, frozen",關島,0,-   ,8618,KGM ,458
    12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",加拿大,0,-   ,0,TNE ,43
    12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",美國,0,-   ,0,TNE ,9
    12019000104,黑豆，不論是否破碎," Black soybeans, whether or not broken",菲律賓,0,-   ,0,TNE ,6
    52114200005,牛仔布, Denim,中國大陸,11398,MTK ,1991,KGM ,902
    52114200005,牛仔布, Denim,日本,14364,MTK ,3898,KGM ,1596
    52114200005,牛仔布, Denim,印尼,21998,MTK ,3869,KGM ,1543
    52114200005,牛仔布, Denim,印度,7212,MTK ,2185,KGM ,513
    52114200005,牛仔布, Denim,柬埔寨,28081,MTK ,9915,KGM ,2469
    52114200005,牛仔布, Denim,馬來西亞,8925,MTK ,3598,KGM ,575
    52114200005,牛仔布, Denim,越南,139191,MTK ,53225,KGM ,12330
    52114200005,牛仔布, Denim,賴索托,6894,MTK ,2771,KGM ,435
    


```python
with open("sample.csv","r",encoding="utf-8") as inFile:
    _data = inFile.readlines()
# print(_data)


_data = _data[1:]

valueSum = 0

### getValue 
for w in _data:
    value = w.strip().split(",")[-1]
    
    valueSum += int(value)
    print(value)

print("="*50)
print("Sum : ",valueSum)

```

    411
    696
    7365
    24919
    729
    1274
    6128
    46022
    2
    4786
    458
    43
    9
    6
    902
    1596
    1543
    513
    2469
    575
    12330
    435
    ==================================================
    Sum :  113211
    


```python
### Read data
def readData(fileName):
    with open(fileName,"r",encoding="utf-8") as inFile:
        _data = inFile.readlines()
        
    return _data


### get value sum     
def getValueSum(data):
    valueSum = 0

    for w in data:
        value = w.strip().split(",")[-1]

        valueSum += int(value)
        
    return valueSum


# main 
    
_data = readData("sample.csv")

_data = _data[1:]

valueSum = getValueSum(_data)

print("Sum : ",valueSum)

```

    Sum :  113211
    


```python

```
