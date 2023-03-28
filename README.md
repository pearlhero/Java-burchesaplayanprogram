# Java-burchesaplayanprogram
Java-burchesaplayanprogram

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner giris = new Scanner(System.in);
        int ay,gun;
        String burc = null;
        System.out.println("Burç Hesaplama");
        System.out.print("Lütfen ay giriniz(1 ile 12 arasında)= ");
        ay = giris.nextInt();

        while(ay<1||ay>12){
            System.out.print("Lütfen ay giriniz(1 ile 12 arasında)= ");
            ay=giris.nextInt();
        }
        System.out.print("Lütfen gün giriniz(1den 31e kadar)= ");
        gun=giris.nextInt();
        while(gun<1||gun>31){
            System.out.print("Lütfen gün giriniz(1den 31e kadar)= ");
            gun=giris.nextInt();
        }
        if(ay == 1){
            if(gun <= 19){burc = "Oğlak";}
            if(gun > 19){burc = "Kova";}
        }
        if(ay == 2){
            if(gun <= 18){burc = "Kova";}
            if(gun > 18){burc = "Balık";}
        }
        if(ay == 3){
            if(gun <= 19){burc = "Balık";}
            if(gun > 19){burc = "Koç";}
        }
        if(ay == 4){
            if(gun <= 19){burc = "Koç";}
            if(gun > 19){burc = "Boğa";}
        }
        if(ay == 5){
            if(gun <= 20){burc = "Boğa";}
            if(gun > 20){burc = "İkizler";}
        }
        if(ay == 6){
            if(gun <= 21){burc = "İkizler";}
            if(gun > 21){burc = "Yengeç";}
        }
        if(ay == 7){
            if(gun <= 22){burc = "Yengeç";}
            if(gun > 22){burc = "Aslan";}
        }
        if(ay == 8){
            if(gun <= 22){burc = "Aslan";}
            if(gun > 22){burc = "Başak";}
        }
        if(ay == 9){
            if(gun <= 22){burc = "Başak";}
            if(gun > 22){burc = "Terazi";}
        }
        if(ay == 10){
            if(gun <= 22){burc = "Terazi";}
            if(gun > 22){burc = "Akrep";}
        }
        if(ay == 11){
            if(gun <= 21){burc = "Akrep";}
            if(gun > 21){burc = "Yay";}
        }
        if(ay == 12){
            if(gun <= 21){burc = "Yay";}
            if(gun > 21){burc = "Oğlak";}
        }
        System.out.print("Burcunuz:" + burc);
    }
}
