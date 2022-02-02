# 02.02.2022
                                                                              ОТЧЁТ.
Задача 1. Дано два числа a и b. Выведите гипотенузу треугольника с заданными катетами.
Входные данные
Вводятся два целых положительных числа, не превышающих 1000.
Выходные данные
Выведите ответ на задачу с точностью 10 знаков после запятой. 
Решение : a=int(input())
b=int(input())
c=(a**2+b**2)**0.5
print(c)
Задача 2. Напишите программу, которая приветствует пользователя, выводя слово Hello, введенное имя и знаки препинания по образцу (см. пример входных и выходных данных). Программа должна считывать в строковую переменную значение и писать соответствующее приветствие. Обратите внимание, что после запятой должен обязательно стоять пробел, а перед восклицательным знаком пробела нет.
Входные данные
Вводится строка, длина которой не превышает 100 символов.
Выходные данные
Выведите ответ на задачу.
Решение : a=input()
print('Hello,',a+'!')
Задача 3. Напишите программу, которая считывает целое число и выводит текст, аналогичный приведенному в примере (пробелы важны!):
Входные данные
Вводится целое число (гарантируется, что число находится в диапазоне от -1000 до +1000).
Выходные данные
Выведите две строки, согласно образцу.
Решение. n= int(input())
print ('The next number for the number', n,'is',str(n+1)+'.')
print ('The previous number for the number',n,'is',str(n-1)+'.')
Задача 4. n  школьников делят k яблок поровну, неделящийся остаток остается в корзинке. Сколько яблок достанется каждому школьнику?
Входные данные
Программа получает на вход числа n и k - целые, положительные, не превышают 10000.
Решение. n = int(input())
k = int(input())
print(k//n)
Задача 5.n  школьников делят k яблок поровну, неделящийся остаток остается в корзинке. Сколько яблок останется в корзинке?
Входные данные
Программа получает на вход числа n и k - целые, положительные, не превышают 10000.
Решение.n = int(input())
k = int(input())
print(k%n)
Задача 6.Длина Московской кольцевой автомобильной дороги — 109 километров. Байкер Вася стартует с нулевого километра МКАД и едет со скоростью v километров в час. На какой отметке он остановится через t часов?
Без использования условных операторов эту задачу существенно проще решить языке Python, чем на других языках программирования. Это связано с особенностями реализации целочисленных операций над отрицательными числами.
Входные данные
Программа получает на вход значение v и t. Если v>0, то Вася движется в положительном направлении по МКАД, если же значение v<0, то в отрицательном. (Гарантируется, что исходные числа - целые и находятся в промежутке от -1000 до +1000).
Решение. v = int(input())
t = int(input())
a = v * t
n = a // 109
print(-(109 * n - a))
Выходные данные
Программа должна вывести целое число от 0 до 108 — номер отметки, на которой остановится Вася.
Решение.v = int(input())
t = int(input())
a = v * t
n = a // 109
print(-(109 * n - a))
Задача 7. Дано натуральное число. Выведите его последнюю цифру.
Входные данные
Вводится единственное число (гарантируется, что оно не превышает 10000).
Выходные данные
Выведите ответ на задачу.
Решение. a = int(input())
print(a%10)
Задача 8. Дано двузначное число. Найдите число десятков в нем.
Входные данные
Вводится единственное число (гарантируется, что оно соответствует условию задачи).
Выходные данные
Выведите ответ на задачу.
Решение. a = int(input())
print(a//10)
Задача 9. Дано натуральное число. Найдите число десятков в его десятичной записи.
Входные данные
Вводится единственное число (гарантируется, что число не превышает 106).
Выходные данные
Выведите ответ на задачу.
a = int(input())
print(a//10)
Задача 10. Дано трехзначное число. Найдите сумму его цифр.
Входные данные
Вводится целое положительное число. Гарантируется, что оно соответствует условию задачи.
Выходные данные
Выведите ответ на задачу.
Решение. a = int(input())
b = a // 100
c = a % 100 // 10
d = a % 10
print(b + c + d)
Задача 11.Дано целое число n. Выведите следующее за ним четное число.
Задачу необходимо решить целочисленными операциями без использования условных операторов (в том числе без тернарного оператора ?: в С++) и\или циклов.
Входные данные
Вводится целое положительное число, не превышающее 1000.
Выходные данные
Выведите ответ на задачу.
Решение.n = int(input())
print((n//2+1)*2)
Задача 12. Обувная фабрика собирается начать выпуск элитной модели ботинок. Дырочки для шнуровки будут расположены в два ряда, расстояние между рядами равно a, а расстояние между дырочками в ряду b. Количество дырочек в каждом ряду равно N. Шнуровка должна происходить элитным способом “наверх, по горизонтали в другой ряд, наверх, по горизонтали и т.д.” (см. рисунок). Кроме того, чтобы шнурки можно было завязать элитным бантиком, длина свободного конца шнурка должна быть l. Какова должна быть длина шнурка для этих ботинок?
Входные данные
Программа получает на вход четыре натуральных числа a, b, l и N.
Выходные данные
Программа должна выводить одно число – искомую длину шнурка. 
Решение . a = int(input())
b = int(input())
l = int(input())
N = int(input())
print((a*2+b*2)*(N-1)+l*2+a)
Задача 13.В некоторой школе решили набрать три новых математических класса и оборудовать кабинеты для них новыми партами. За каждой партой может сидеть два учащихся. Известно количество учащихся в каждом из трех классов. Выведите наименьшее число парт, которое нужно приобрести для них.
Входные данные
Программа получает на вход три неотрицательных числа: количество учащихся в каждом из трех классов (числа не превышают 1000).
Выходные данные
Выведите ответ на задачу.
Решение.a = int(input())
b = int(input())
c = int(input())
print(a // 2 + b // 2 + c // 2 + a % 2 + b % 2 + c % 2)
Задача 14. Дано число n. С начала суток прошло n минут. Определите, сколько часов и минут будут показывать электронные часы в этот момент.
Входные данные
Вводится число n - целое, положительное, не превышает 107.
Выходные данные
Программа должна вывести два числа: количество часов (от 0 до 23) и количество минут (от 0 до 59).
Учтите, что число n может быть больше, чем количество минут в сутках.
Решение.n = int(input())
a = n % (60 * 24) // 60
b = n % 60
print(a, b)
Задача 15.Электронные часы показывают время в формате h:mm:ss, то есть сначала записывается количество часов в диапазоне от 0 до 23, потом обязательно двузначное количество минут, затем обязательно двузначное количество секунд. Количество минут и секунд при необходимости дополняются до двузначного числа нулями.
С начала некоторых суток прошло n секунд. Выведите, что покажут часы. Задачу необходимо решить без использования условных операторов (в том числе без тернарного оператора ?: в С++) и\или циклов.
Входные данные
Вводится число n - целое, положительное, не превышает 107.
Выходные данные
Выведите показания часов, соблюдая формат.
Решение. n = int(input())
if n<86400:
    print (n//3600)
    print (n//60)
    print (n%60)
else:
    print ((n % 86400) // 3600)
    print ((n % 86400) // 60)
    print ((n % 86400) % 60)
Задача 16. Напишите программу, которая считывает значения двух переменных a и b, затем меняет их значения местами (то есть в переменной a должно быть записано то, что раньше хранилось в b, а в переменной b записано то, что раньше хранилось в a). Затем выведите значения переменных.
Входные данные
Вводятся два целых числа (гарантируется, что числа находятся в промежутке от -1000 до +1000).
Выходные данные
Выведите ответ на задачу.
Примечание
Решением задачи не является такой код:
ввод (a)
ввод (b)
вывод (b, a)
Решение. a = int(input())
b = int(input())
t = a
a = b
b = t
print(a, b)
