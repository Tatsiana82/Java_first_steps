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
# Lesson_3 Задача №1 HW_3
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
#Lesson_4 Задача №1 Необходимо вывести числа от 0 до 15. HW_4
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
#Lesson 5 HW_5
Задача №1
Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести сумму всех значений массива.
public class Arrays {
    public static void main(String[] args) {
        int[] arr = {9, 2, 6, 4, 5, 12, 7, 8, 6};

        int sum = 0;
        int min = Integer.MAX_VALUE;
        for (int i = 0; i < arr.length; i++){

                sum += arr[i];
            }

        System.out.println(sum);
    }
}
**********************************************************************************************************

Задача №2

Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести максимальное значение массива.
public class Arrays2 {
    public static void main(String[] args) {
        int[] arr = {9, 2, 6, 4, 5, 12, 7, 8, 6};
        int max = Integer.MIN_VALUE;
        for (int i = 0; i < arr.length; i = i + 1){
            if (arr[i] > max) {
                max = arr[i];
            }
        }
        System.out.println(max);
    }
}
*************************************************************************************
Задача №3

Дан массив:
int[] array = {9, 2, 6, 4, 5, 12, 7, 8, 6};
необходимо вывести минимальное значение массива.
public class Arrays2 {
    public static void main(String[] args) {
        int[] arr = {9, 2, 6, 4, 5, 12, 7, 8, 6};
        int min = Integer.MAX_VALUE;
        for (int i = 0; i < arr.length; i = i + 1){
            if (arr[i] < min) {
                min = arr[i];
            }
        }
        System.out.println(min);
    }
}
*******************************************************************************************
Задача №4

Дан массив:
int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9};
необходимо вывести среднее арифметическое всех значений массива.

public class Arrays3 {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9};
        double sum = 0;

        for (int i = 0; i < array.length; i++) {
            sum += array[i];
        }

        System.out.println(sum / array.length);
    }
}
*********************************************************************************************************************
Задача №5

Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести сумму элементов массива.

public class Arrays3 {
    public static void main(String[] args) {
        int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
        int sum = 0;

        for (int i = 0; i < array.length; i++) {
            for (int j = 0; j < array[i].length; j++) {
                sum += array[i][j];
            }
        }
        System.out.println(sum);
    }
}
**********************************************************************************************************************
Задача №6

Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести максимальное значение массива.

public class Arrays4 {
    public static void main(String[] args) {
        int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};

        int max = Integer.MIN_VALUE;
        for (int i = 0; i < array.length; i++) {
            for (int j = 0; j < array[i].length; j++) {
                if (array[i][j] > max) {
                    max = array[i][j];
                }
            }
        }
        System.out.println(max);
    }
}
*****************************************************************************************************************

Задача №7

Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести количество элементов в массиве.

public class Arrays5 {

        public static void main(String[] args) {
            int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};

            int count = 0;
            for (int i = 0; i < array.length; i++) {
                for (int j = 0; j < array[i].length; j++) {
                   count++;
                }
            }
            System.out.println(count);
        }
    }
************************************************************************************************************

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
******************************************************************************
https://www.codewars.com/kata/555086d53eac039a2a000083/train/java

public class OppositesAttract {

  public static boolean isLove(final int flower1, final int flower2) {
return (flower1 + flower2) % 2!= 0;
  }
  
}
**************************************************************************
https://www.codewars.com/kata/5265326f5fda8eb1160004c8/train/java
class Kata {
  public static String numberToString(int num) {
    // Return a string of the number here!
    return num + "";
  }
}
***********************************************************************
https://www.codewars.com/kata/55a2d7ebe362935a210000b2/train/java

import java.util.Arrays;

public class SmallestIntegerFinder {
    public static int findSmallestInt(int[] args) {
      int min = args[0];
      
       for(int i = 1; i < args.length; i++){
         if(min > args[i]) min = args[i];
       }
       
      return min;
    }
}
****************************************************************************
https://www.codewars.com/kata/5b077ebdaf15be5c7f000077/train/java

class Kata {
  public static String countingSheep(int num) {
    //Add your code here
    String res = "";
    
    for(int i = 0; i < num; i++){
      res += 1 + i + " sheep...";
    }
    return res;
  }
}
*****************************************************************************
# Lesson 7 Задача №1

Задача №1

Необходимо создать класс Person с полями: имя, возраст, пол. Класс должен иметь метод - getName, метод возвращает имя с префиксом “Mr. ” если пол указан как мужской и префикс “Mrs. ” если женский.

public class Main_HW_7 {
    public static void main(String[] args) {
        HW_7_Person man = new HW_7_Person();
        man.name = "Ivan Ivanov";
        man.age = 40;
        man.sex = "m";

        System.out.println(man.getName());

        HW_7_Person woman = new HW_7_Person();
        woman.name = "Lilya Petrova";
        woman.age = 42;
        woman.sex = "f";

        System.out.println(woman.getName());

        HW_7_Person unknown = new HW_7_Person();
        unknown.name = "Rod";
        unknown.age = 152;
        unknown.sex = "x";

        System.out.println(unknown.getName());
    }
}


public class HW_7_Person {

        String name;
        int age;

        String sex;
        //char sex;


        String getName() {
            String prefix = "";
            if (sex == "m") {
                prefix = "Mr. ";
            } else if (sex == "f") {
                prefix = "Mrs. ";
            }
            return prefix + name;
        }

    }

Задача №2

Необходимо создать класс Employee с полями как у Person (из предыдущего задания) и поле зарплата. Класс должен иметь метод isSameName(Employee employee) который возвращает true, если у сотрудника у которого был вызван метод и сотрудника который был передан как параметр, одинаковое имя.

public class Main_HW_7 {
    public static void main(String[] args) {
        Employee john = new Employee();
        john.name = "John Parker";
        john.age = 27;
        john.sex = "m";
        john.salary = 1500.0;

        Employee pete = new Employee();
        pete.name = "Pete Holms";
        pete.age = 33;
        pete.sex = "m";
        pete.salary = 1800.0;

        System.out.println(john.isSameName(pete));

        Employee gjohn = new Employee();
        gjohn.name = "John Parker";
        gjohn.age = 27;
        gjohn.sex = "m";
        gjohn.salary = 2800.0;

        System.out.println(john.isSameName(gjohn));
        
        System.out.println(john.equals(gjohn));

    }
}

public class HW_7_Person {

        String name;
        int age;

        String sex;
        //char sex;

Задача №3

Необходимо создать класс Salary с единственным методом - getSum(Employee[] employeeArray), метод должен возвращать сумму зарплат всех сотрудников из массива переданного в качестве аргумента вызова метода.

public class Main_HW_7 {
    public static void main(String[] args) {
        Employee john = new Employee();
        john.name = "John Parker";
        john.age = 27;
        john.sex = "m";
        john.salary = 1500.0;

        Employee pete = new Employee();
        pete.name = "Pete Holms";
        pete.age = 33;
        pete.sex = "m";
        pete.salary = 1800.0;

   
        Employee gjohn = new Employee();
        gjohn.name = "John Parker";
        gjohn.age = 27;
        gjohn.sex = "m";
        gjohn.salary = 2800.0;

        Employee[] employees = {john,pete, gjohn};

        System.out.println(Salary.getSum(employees));


public class Salary {

    static double getSum(Employee[] employeeArray){
        double result = 0.0;
        for(int i = 0; i < employeeArray.length; i++){
            result += employeeArray[i].salary;

        }
        return result;
    }

}
***************************************************************************************
Lesson_8
Задачи

https://www.codewars.com/kata/playing-with-cubes-i/train/java

public class Cube{

  private int side;
  
  public int getSide(){
    return this.side;
  }
  
  public void setSide(int newSide){
    this.side = newSide;
  }
}

https://www.codewars.com/kata/building-blocks/train/java
public class Block{
	int width;
    int length;
    int height;
    
    Block(int[] arr) {
        this.width = arr[0];
        this.length = arr[1];
        this.height = arr[2];
    }
    int getWidth() {
        return width;
    }
    int getLength() {
        return length;
    }
    int getHeight() {
        return height;
    }
    int getVolume() {
        return getWidth() * getLength() * getHeight();
    }
    int getSurfaceArea() {
        return getWidth() * getLength() * 2 + getHeight() * getLength() * 2 + getWidth() * getHeight() * 2;
    }
}

Экстра задача
https://www.codewars.com/kata/two-fighters-one-winner/java
public class Kata {
  public static String declareWinner(Fighter fighter1, Fighter fighter2, String firstAttacker) {
    Fighter a = fighter1;
    Fighter b = fighter2;
    if (firstAttacker.equals(fighter2.name)) {
      a = fighter2;
      b = fighter1;
    }    
    while (true) {      
      if ((b.health -= a.damagePerAttack) <= 0)
        return a.name;  
      if ((a.health -= b.damagePerAttack) <= 0)
        return b.name;
    }
  }
}
********************************************************************************************************
Lesson_9 HW_9

Задача №1

Создать класс Month с полями: имя месяца, количеством дней и количеством рабочих дней. Создать класс MonthUtils который бы хранил подготовленные месяцы или их массивы для использования (объекты класса Month).


Задача №2

Необходимо создать класс Employee с полями: имя, возраст, пол и ЗП в день. Все поля сделать приватными и для каждого поля добавить методы set и get. Класс должен иметь метод - getSalary(Month[] monthArray), метод возвращает зарплату за те месяцы которые были переданы в качестве аргумента.


Задача №3

Необходимо создать класс Manager с полями: имя, возраст, пол, ЗП в день и количество подчиненных. Все поля сделать приватными и для каждого поля добавить методы set и get. Класс должен иметь метод - getSalary(Month[] monthArray), метод возвращает зарплату за те месяцы которые были переданы в качестве аргумента.
К рассчитанной ЗП должно прибавляться по 1% за каждого подчиненного.


Задача №4 (*)

Для учета автомобилей на дороге важно, чтобы номера не повторялись. Необходимо создать класс LicensePlate, в котором есть неизменяемое строковое поле plate. Запретить создавать экземпляры этого класса кому попало (т.е. классам за пределами того пакета/package, в котором находится класс LicensePlate).
Для выдачи номеров создать класс LicensePlateMaker, который хранит в себе неизменяемый префикс (например, CA для Калифорнии или NY для Нью-Йорка)  и имеет метод makeNextPlate(), который создает новые номера формата “CA-1”, “CA-2”, “CA-123” по порядку. Или “NY-300”, “NY-301” и т. д.
Номера, конечно же, повторяться не должны, хотя бы на период существования данного экземпляра класса LicensePlateMaker.

(обращаю внимание, эта задача — со звездочкой)
*****************************************************************************************************************
Lesson_10 HW_10
Задача №1

Необходимо создать класс Employee со следующими методами: 
getBaseSalary - получить базовую ставку
setBaseSalary
getName - получить имя
setName
getSalary - получить зарплату


Задача №2

Необходимо создать класс Worker где метод getSalary будет возвращать базовую ставку.

Необходимо создать класс Manager в который нужно добавить следующие методы:
getNumberOfSubordinates - получить количество подчиненных
setNumberOfSubordinates

 в классе, метод getSalary будет возвращать значение по формуле - <базовая ставка> * (<количество подчиненных> / 100 * 3). Если количество подчиненных 0, то результат как у обычного рабочего.

Необходимо создать класс Director с теми же методами, что и Manager, но метод getSalary должен возвращать результат по формуле - <базовая ставка> * (<количество подчиненных> / 100 * 9). Если количество подчиненных 0, то результат как у обычного рабочего.


Задача №3

Необходимо создать утилитарный класс со следующими методами:
поиск сотрудника в массиве по его имени
поиск сотрудника в массиве по вхождению указанной строки в его имени
подсчет зарплатного бюджета для всех сотрудников в массиве
поиск наименьшей зарплаты в массиве
поиск наибольшей зарплаты в массиве
поиск наименьшего количества подчиненных в массиве менеджеров
поиск наибольшего количества подчиненных в массиве менеджеров
поиск наибольшей надбавки (разнице между базовой ставкой и зарплатой) в массиве менеджеров
поиск наименьшей надбавки (разнице между базовой ставкой и зарплатой) в массиве менеджеров



