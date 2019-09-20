# belajar
package latarray;

import java.util.Scanner; public class LatPrak1 {

public static void main(String[] args) {
   String carii;
   boolean found = false;
   String[] nama = new String [] {"gala","raka","abdi","iwan","lucky"};
   Scanner input = new Scanner(System.in);
    System.out.println("lebkno nama sng pingin di goleki ");
    carii = input.nextLine();
    for (int i =0; i < nama.length; i++) {
        if(carii.equalsIgnoreCase(nama[i])) {           
            found = true;
            break;
       }
    }
    if (found == true) {
        System.out.println("datane ono lur");
    }else{
        System.out.println("datane ganok lur");
    }
}
}

package latarray;

import java.util.Scanner;

public class LatPrak2 {

public static void main(String[] args) {
    int cari;
    boolean found = false;
    int[] data = new int[]{8, 90, 56, 90, 87, 76, 42};
    Scanner input = new Scanner(System.in);
    System.out.println("lebkno data sng pingin di goleki (1-10)");
    cari = input.nextInt();
    for (int i = 0; i < data.length; i++) {
        if (cari == data[i]) {
            found = true;
            System.out.println("data ono,urutan ke-" + i);
        }
    }
    if (found == true) {
        System.out.println("datane ono lur");
    } else {
        System.out.println("datane ganok lur");
    }
}
}

package latarray;

public class LatPrak3 {

public static void main(String[] args) {
    int min = 0;
    int[] data = new int[]{-21, 82, 0, 19, -83, 10,};
    System.out.println("data pada aarray");
    for (int i = 0; i < data.length; i++) {
        System.out.println(data[i] + "\t");
        if (data[i] > min) {
            min = data[i];
        }
    }
    System.out.println("\n data terbesar dari array adalah " + min);
}
}

package latarray;

import java.util.Scanner;

public class LatPrak4 {

public static void main(String[] args) {
    Scanner input = new Scanner(System.in);
    String cari;
    System.out.println("masukkan kata/kalimat: ");
    cari = input.nextLine();

    int a = 0;
    for (int i = 0; i < cari.length(); i++) {
        if (cari.charAt(i) == 'a') {
            a++;
        }
    }
    System.out.println("Jumlah hurufa pada kalimat di atas adalah " + a);
}
}

package latarray;

import java.util.Scanner;

public class Tugas1 {

public static void main(String[] args) {
    int cari = 0;
    int bilangan;
    boolean ditemukan = false;
    int data[] = {74, 98, 72, 74, 72, 90, 81, 72};
    Scanner input = new Scanner(System.in);
    System.out.println("Data pada array");
    for (int i = 0; i < data.length; i++) {
        System.out.print(data[i] + "\t");
    }
    System.out.println("\nmasukkan nilai yang dicari: ");
    bilangan = input.nextInt();
    int oke = 0;
    for (int i = 0; i < data.length; i++) {
        if (data[i] == bilangan) {
            oke++;
            ditemukan = true;
        }
    }
    if (ditemukan == true) {
        System.out.println("Data yang dicari di atas ditemukan sebanyak " + oke + " kali");

    } else {
        System.out.println("Data tidak ditemukan");
    }

}
}

package latarray;

public class Tugas2 {

public static void main(String[] args) {

    int a = 0;
    int nilai[] = new int[]{76, 60, 90, 86};
    double ratarata = 0;
    System.out.println("Data pada array");
    for (int i = 0; i < nilai.length; i++) {
        System.out.print(nilai[i] + "\t");
        ratarata += nilai[i];

    }
    ratarata /= nilai.length;
    System.out.println("\n");
    System.out.println("Nilai Rata Rata : " + ratarata);
    for (int i = 0; i < nilai.length; i++) {
        if (ratarata < nilai[i]) {
            a++;

        }
    }
    System.out.println("Siswa Yang Lulus Sebanyak : " + a);
    for (int i = 0; i < nilai.length; i++) {
        if (ratarata < nilai[i]) {
            int x = nilai[i];
            System.out.println("Siswa yang memiliki nilai : " + x);

        }

    }
}
}

package latarray;

public class Tugas3 {

public static void main(String[] args) {

    int cari = 3;
    int a = 0;
    int nilai[] = new int[]{92, 98, 76, 72, 81, 101, 39};
    System.out.println("Data pada array");
    for (int i = 0; i < nilai.length; i++) {
        System.out.print(nilai[i] + "\t");

    }
    System.out.println("\n" + "Bilangan yang kelipatan 3 :");
    for (int i = 0; i < nilai.length; i++) {
        if (nilai[i] % 3 == 0) {
            int x = nilai[i];

            System.out.println(+nilai[i]);
        }

    }

}
}

package latarray;

import java.util.Scanner;

public class Tugas4 {

public static void main(String[] args) {

    Scanner scan = new Scanner(System.in);
    String cari;
    System.out.print("Masukkan kata : ");
    cari = scan.nextLine();
    int a = 0, b = 0, c = 0, d = 0, e = 0;
    for (int i = 0; i < cari.length(); i++) {
        if (cari.charAt(i) == 'a') {
            a++;
        }
        if (cari.charAt(i) == 'i') {
            b++;
        }
        if (cari.charAt(i) == 'u') {
            c++;
        }
        if (cari.charAt(i) == 'e') {
            d++;
        }
        if (cari.charAt(i) == 'o') {
            e++;
        }
    }
    int f = a + b + c + d + e;
    System.out.println("Jumlah huruf a pada kata yang ditulis adalah : " + a);
    System.out.println("Jumlah huruf i pada kata yang ditulis adalah : " + b);
    System.out.println("Jumlah huruf u pada kata yang ditulis adalah : " + c);
    System.out.println("Jumlah huruf e pada kata yang ditulis adalah : " + d);
    System.out.println("Jumlah huruf o pada kata yang ditulis adalah : " + e);
    System.out.println("Jumlah huruf vokal :" + f);

}
}
