import java.util.Scanner;
// Calculator
public class Main {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        System.out.println("Введите число 1: ");
        int a = scanner.nextInt();
        System.out.println("Введите число 2: ");
        int b = scanner.nextInt();

        System.out.printf("Введите операцию: "); // +  -  /  *  **  %
        String operations = scanner.next();

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










import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        System.out.println("Оценка 1-предмета за семемстр: ");
        int Math = scanner.nextInt();

        System.out.println("Оценка 2-предмета за семемстр: ");
        int Physics = scanner.nextInt();

        System.out.println("Оценка 3-предмета за семемстр: ");
        int English = scanner.nextInt();

        double avarage = (Math + Physics + English) / 3;
        System.out.println("Средняя оценка за семестр: " + avarage);

        if (Math <= 49 || Physics < 50 ||49 English < 50)
            System.out.println("Надо было учиться :( ");
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
