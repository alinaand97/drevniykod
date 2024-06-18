# Слишком древний шифр
list = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]
para=[]
vvod=int(input("Введите чисило от 3 до 20: "))


for i in range(1, len(list)):
    for j in range(2, len(list)):
        if (vvod % (int(i) + int(j)) == 0 and i!=j):
            if not ([j, i] in para ) :
                para.append([i, j])

print(para)
