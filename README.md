# software-enginering
public class 冒泡排序 {

    public int[] bubbleSort(int[] a, int n) {

        for (int i = 0; i < n; i++) {

            int flag = 0;

            for (int j = n - 1; j > i; j--) {

                if (a[j] < a[j - 1]) {

                    int x = a[j];

                    a[j] = a[j - 1];

                    a[j - 1] = x;

                    flag = 1;

                }

            }

            if (flag == 0)

                break;

        }

        return a;

    }
    
    public static void main(String[] args) {

        int[] a = new int[] { 25, 56, 32, 20, 1, 5, 89, 3, 8, 41 };

        冒泡排序 sort = new 冒泡排序();

        sort.bubbleSort(a, a.length);

        for (int i = 0; i < a.length; i++) {

            System.out.print(a[i] + " ");

        }

    }

}
