# Hello-word
Lesson one
public class Example_17 {
    public static void main(String[] args) {
        int[] mas = {1, 2, 3, 5, 3, 2, 3, 2, 1, 1, 2, 4};
        int countMas = 0;

        int thisMas = 0;
        int indexBigMasCount = 0;

        for (int i = 1 ; i < mas.length; i++) {
            for (int j = 0; j < mas.length; j++) {
                if (mas[i] == mas[j]) {
                    countMas++;/*нашел значения равное i=j, потом добавил 1 */
                }
            }
            if (thisMas < countMas) {
                thisMas = countMas;
                indexBigMasCount = i;
            }
            countMas = 0;
        }
        System.out.println("Больше всего " + mas[indexBigMasCount]);
    }
}
