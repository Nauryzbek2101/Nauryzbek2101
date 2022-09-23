import java.util.Scanner;

public class Main {
    public static void main(String[] args) {


        int Math = 70;
        System.out.println("Оценка 1-предмета за семемстр: " + Math);

        int Physics = 85;
        System.out.println("Оценка 2-предмета за семемстр: " + Physics);

        int English = 95;
        System.out.println("Оценка 3-предмета за семемстр: " + English);

        double avarage = (Math + Physics + English) / 3;
        System.out.println("Средняя оценка за семестр: " + avarage);

        if (Math <= 49 || Physics < 50 ||  English < 50){
            System.out.println("Надо было учиться :( ");}
        else if (avarage >= 50 && avarage <= 69)
            System.out.println("Ты слетел со стипендии :( ");
        else if (avarage >= 70)
            System.out.println("Ты не слетел со стипендии!");
        else if (avarage <= 49)
            System.out.println("RETAKE!");
        else
            System.out.println("Всё зависет от тебя!");

    }
}



import java.util.Scanner;
// Calculator
public class Main {
    public static void main(String[] args) {

        int a = 46;
        System.out.println("Число 1: " + a);

        int b = 54;
        System.out.println("Число 2: " + b);

        String operations = "*";

        switch (operations){
            case "+":
                System.out.println(a + b);
                break;
            case "-":
                System.out.println(a - b);
                break;
            case "**":
                System.out.println((int)Math.pow(a, b));
                break;
            case "/":
                System.out.println(a / b);
                break;
            case "*":
                System.out.println(a * b);
                break;
            default:
                System.out.println("Вы ввели не понятную операцию!");
        }
    }
}
