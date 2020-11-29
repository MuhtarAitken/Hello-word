# Hello-word
Lesson one
import java.util.Scanner;

public class Example_16 {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);// Scaner scaner = new Scaner (System.in)
        int[] mas={1, 4, 6};
        System.out.println("Значения массива: ");
        for (int i=0; i < mas.length; i++) {
            System.out.println(mas[i]);
        }

        System.out.println("Введите значения нужного элемента:");
        int masValue=scanner.nextInt();
        boolean isFind=false;
        int masIndex=0;
        String message=" ";
        for (int i=0; i < mas.length; i++) {
            if (mas[i] == masValue) {
                isFind=true;
                masIndex=i;
            }
        }
        if (isFind == true) {
            message="нужный элемент" + ", его индекс " + masIndex;
        } else {
            message="-1";
        }
        System.out.println(message);
    }
}
