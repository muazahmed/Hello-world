/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package home;

import java.util.Scanner;

/*
 *
 * @author moaaz
 */
public class Deneme {
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner scan=new Scanner(System.in);
        System.out.print("Please enter you number to get it's fibonaci : ");
        long k=fibonaci(scan.nextLong());
        System.out.println(k);
    }
    static long fibonaci(long sayi){
        long a = 0,b=1,toplam=0;
        for (int i = 0; i < sayi; i++) {
            toplam=a+b;
            a=b;
            b=toplam;
        }
        return toplam;
    }
}
