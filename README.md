# UKLsoal11[UjianUKLkenaikanLEvel.java](https://github.com/user-attachments/files/23922728/UjianUKLkenaikanLEvel.java)
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ujianuklkenaikanlevel;

import java.util.Scanner;

/**
 *
 * @author Danielrorrrrr
 */
public class UjianUKLkenaikanLEvel {

    public static void main(String[] args) {
         Scanner masukkan = new Scanner(System.in);

        System.out.print("Masukkan sebuah bilangan : ");
        int bilangan = masukkan.nextInt();

        boolean prima = true;

        if (bilangan <= 1) {
            prima = false;
        } else {
            for (int i = 2; i <= bilangan / 2; i++) {
                if (bilangan % i == 0) {
                    prima = false;
                    break;
                }
            }
        }

        if (prima) {
            System.out.println(bilangan + " Bilangan prima");
        } else {
            System.out.println(bilangan + " Bukan bilangan prima");
        }
    }
}
       
    
