# Java_first_steps
# What do you need for complete happiness? Of course, try to learn the Java language. Java is a Jumanji game, you start to discover it and it pulls you into the unknown. Enjoy Java!
*****************************************************************************************************************************
#Lesson_1_HW
Задача №1 Написать программу которая будет печатать/выводить следующий текст:
3
2
1
Поехали!!!
*****************************************************************************************************************************
Code:
public class First1 {

    public static void main(String[] args) {
        System.out.println("""
        3
        2
        1
        Поехали!!!""");
    }
}
*****************************************************************************************************************************
#Lesson_2 Задача №1

Необходимо создать целочисленные переменные a и b, присвоить произвольные значения переменным на ваш выбор и вывести результаты следующих операций с этими переменными: 
сложение; addition; +
умножение; multiplication; *
вычитание; subtraction; -
деление; division; /
остаток от деления. the remainder of the division. %
Так же сделать проверку на четность этих переменных и вывести результат.
*****************************************************************************************************************************
public class Operators {
    public static void main(String[] args) {
        int a = 12;
        int b = 7;
        System.out.println(a + b);
        System.out.println(a - b);
        System.out.println(a * b);
        System.out.println(1.0 * a / b);
        System.out.println(a % b);
        System.out.println("even" + " " + a % 2);
        System.out.println("odd" +  " " + b % 2);

    }
}
***********************************************************************************************************************
# Lesson_3 Задача №1
Необходимо создать две целочисленные переменные (a, b), присвоить произвольные значения переменным на ваш выбор и вывести следующие строки: 
a == b - если переменные равны
a < b - если переменная a меньше b
a > b - если переменная b меньше a
**********************************************************************************************************************
public class operators_cond {
            public static void main(String[] args) {
            int a = 25;
            int b = 10;

            if (a == b) {
                System.out.println("a == b");
            } else if (a < b) {
                System.out.println("a < b");
            } else {
                System.out.println("a > b");
            }
        }
    }
    *****************************************************************************************************************
#Задача №2
Необходимо создать две целочисленные переменные (a, b), присвоить произвольные значения переменным на ваш выбор и вывести следующие строки: 
maybe a and b are even - если сумма переменных четная
some variable is odd - если сумма переменных нечетная
*******************************************************************************************************************
public class operations_cond_2 {
    public static void main(String[] args) {
        int a = 5;
        int b = 20;

        if ((a + b) % 2 == 0){
        System.out.println("maybe a and b are even");

} else {
        System.out.println("odd");
    }
    }
    }

*******************************************************************************************************************
#Задача №3
Необходимо создать целочисленную переменную, присвоить произвольное значение переменной на ваш выбор и вывести следующие строки: 
больше 10 - если переменная больше 10
меньше 100 - если переменная меньше 100
результат деления на 2 больше 20 - если это соответствует истине
значение переменной между 5 и 40 включительно - если это правда
значение переменной меньше 5 или больше 40 - если предыдущие условие ложное
*********************************************************************************************************************
public class operators_cond_3 {
    public static void main(String[] args) {
        int a = 45;
        if (a > 10) {
            System.out.println("больше 10");
        }
        if (a < 100) {
            System.out.println("меньше 100");
        }
        if (a * 1.0 / 2 > 20) {
            System.out.println("результат деления на 2 больше 20");
        }
        if (a > 5 && a <= 40) {
            System.out.println("значение переменной между 5 и 40 включительно");
        }
        else if (a < 5 || a > 40) {
            System.out.println("значение переменной меньше 5 или больше 40");
        }
    }
}
**********************************************************************************************************************
#Lesson_4 Задача №1 Необходимо вывести числа от 0 до 15.
public class HW4 {
    public static void main(String[] args) {
        for (int i = 0; i < 15; i = i + 1){
            System.out.println(i);
        }
    }
}
*******************************************************************************************************************
#Задача №2 Необходимо вывести все положительные степени числа 5 которые меньше 10000, вывести результат возведения в степень.
public class HW4 {
    public static void main(String[] args) {
        for (int i = 5; i < 10000; i = i * 5){
            System.out.println(i);
        }
    }
}
******************************************************************************************************************
#Задача №3
Необходимо вывести все числа кратные 4 между числами 40 и 60 включительно.
Реализовать 2 варианта: 
использовать конструкцию if для определения кратности (цикл с шагом 1, i = i + 1);
без использования конструкции if (шаг цикла на ваше усмотрение).

public class HW4 {
    public static void main(String[] args) {
        for (int i = 40; i <= 60; i = i + 1) {
            if (i % 4 == 0) {
                System.out.println(i);
            }
        }
    }
}
******************************************************************************************************************
# Arrays
Задача №1

Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести все нечетные числа из массива.

import java.util.Arrays;
public class HW4a {
    public static void main(String[] args) {
        int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
        for (int i = 0; i < array.length; i = i + 1) {
            if (array[i] % 2 == 1) {

                System.out.println(array[i]);
            }
        }
    }
}
***************************************************************************************************************
#Задача №2
Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести все значения массива больше 5.

import java.util.Arrays;
public class HW4a {
    public static void main(String[] args) {
        int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
        for (int i = 5; i < array.length; i = i + 1) {
            if (array[i] > 5) {

                System.out.println(array[i]);
            }
        }
    }
}

**************************************************************************************************************
#Задача №3
Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо увеличить все значения массива на 15.

import java.util.Arrays;
public class HW4a {
    public static void main(String[] args) {
        int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
        for (int i = 0; i < array.length; i = i + 1) {
            array[i] = array[i] + 15;


                System.out.println(array[i]);
            }
        }
    }
*************************************************************************************************************
#Lesson 5 
Задача №1
Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести сумму всех значений массива.


Задача №2

Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести максимальное значение массива.


Задача №3

Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести минимальное значение массива.


Задача №4

Дан массив:
int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9};
необходимо вывести среднее арифметическое всех значений массива.


Задача №5

Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести сумму элементов массива.


Задача №6

Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести максимальное значение массива.

Задача №7

Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести количество элементов в массиве.

Вывести следующие строки с соответствующим форматированием (как пирамиды):


Задача №1

0  1  2  3  4  5  6  7  8  9
0  1  2  3  4  5  6  7  8
0  1  2  3  4  5  6  7
0  1  2  3  4  5  6
0  1  2  3  4  5
0  1  2  3  4
0  1  2  3
0  1  2
0  1
0


Задача №2

0  1  2  3  4  5  6  7  8  9
    0  1  2  3  4  5  6  7  8
        0  1  2  3  4  5  6  7
             0  1  2  3  4  5  6
                 0  1  2  3  4  5
                     0  1  2  3  4
                         0  1  2  3
                             0  1  2
                                 0  1
                                     0


Задача №3

9 8 7 6 5 4 3 2 1 0 1 2 3 4 5 6 7 8 9
   8 7 6 5 4 3 2 1 0 1 2 3 4 5 6 7 8
      7 6 5 4 3 2 1 0 1 2 3 4 5 6 7
         6 5 4 3 2 1 0 1 2 3 4 5 6
            5 4 3 2 1 0 1 2 3 4 5
               4 3 2 1 0 1 2 3 4
                  3 2 1 0 1 2 3
                     2 1 0 1 2
                        1 0 1
                           0
************************************************************************************************************************************
#Lesson 6
Задача №1

Дана строка: 
String s = “Перестановочный алгоритм быстрого действия”;
необходимо вывести все буквы “о” из этой строки.
Для указанной строки ответ будет “ооооо” (или в столбик)


Задача №2

Дана строка:
String s = “Перевыборы выбранного президента”;
необходимо подсчитать количество букв “е” в строке.
Для указанной строки ответ будет 4.


Задача №3

Дан массив:
String[][] array = {{“Привет”, “всем”, “кто”}, {“изучает”, “язык”, “программирования”}, {“java”}};
необходимо подсчитать количество строк в массиве, которые не содержат буквы “е”.


Экстра задача

Дана строка:
String s = “Посмотрите как Рите нравится ритм”;
необходимо вывести индексы начала всех подстрок - “рит”, независимо от регистра.
Для указанной строки ответ будет 6, 15, 29.

Задача №1

Необходимо написать 4 метода:
сложение 2х чисел
вычитание 2х чисел
умножение 2х чисел
деление 2х чисел

*******************************************************************************
Задачи №2

https://www.codewars.com/kata/53ee5429ba190077850011d4/train/java
class Java {
  public static int doubleInteger(int i) {
    // Double the integer and return it!
    return i;
  }
}
https://www.codewars.com/kata/555086d53eac039a2a000083/train/java
https://www.codewars.com/kata/5265326f5fda8eb1160004c8/train/java
https://www.codewars.com/kata/55a2d7ebe362935a210000b2/train/java
https://www.codewars.com/kata/5b077ebdaf15be5c7f000077/train/java
*********************************************************************************
# Lesson 7 Задача №1

Необходимо создать класс Person с полями: имя, возраст, пол. Класс должен иметь метод - getName, метод возвращает имя с префиксом “Mr. ” если пол указан как мужской и префикс “Mrs. ” если женский.


Задача №2

Необходимо создать класс Employee с полями как у Person (из предыдущего задания) и поле зарплата. Класс должен иметь метод isSameName(Employee employee) который возвращает true, если у сотрудника у которого был вызван метод и сотрудника который был передан как параметр, одинаковое имя.


Задача №3

Необходимо создать класс Salary с единственным методом - getSum(Employee[] employeeArray), метод должен возвращать сумму зарплат всех сотрудников из массива переданного в качестве аргумента вызова метода.



