# Java_first_steps
# What do you need for complete happiness? Of course, try to learn the Java language. Java is a Jumanji game, you start to discover it and it pulls you into the unknown. Enjoy Java!
*****************************************************************************************************************************
#Lesson_1_HW Задача №1
#Написать программу которая будет печатать/выводить следующий текст:
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
# Lesson_2 Задача №1

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
# Lesson_3
# Задача №1

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



