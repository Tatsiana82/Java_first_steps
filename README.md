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



