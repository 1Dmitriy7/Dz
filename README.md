# Dz
reshenie_kv_uravneniya
package ru.levelp;

/**
 * Created by d174m on 25.05.2016.
 */
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        double a;
        double b;
        double c;
        double d;
        double x1;
        double x2;
        System.out.println("Решим уравнение ax^2 + bx + c = 0");
        System.out.println("Введите a: ");
        a = s.nextDouble();
        System.out.println("Введите b: ");
        b = s.nextDouble();
        System.out.println("Введите c: ");
        c = s.nextDouble();
        d = Math.pow(b, 2) - (4 * a * c);
        if (d > 0) {
            x1 = ((-1) * b + Math.sqrt(d)) / (2 * a);
            x2 = ((-1) * b + Math.sqrt(d)) / (2 * a);
            System.out.println("Корни уравнения: x1= " + x1 + ", x2= " + x2);
        }
        else if (d == 0) {
            x1 = (-1) * b / (2 * a);
            System.out.println("Уравнение имеет единственный корень x1, x2 = " + x1);
        }
        else {
            System.out.println("Ошибка. 0 меньше нуля");
        }

    }
}
