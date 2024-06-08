import java.util.Scanner;

public class Main1 {

    public static void main(String[] args) {
     int mesafe,yas,yoltipi,toplampara;
        Scanner input= new Scanner(System.in);

        System.out.print("Lütfen Yaşınızı giriniz: ");
        yas=input.nextInt();

        System.out.print("Lütfen yolculuk tipini seçiniz 1- Tek yön 2-Çift yön: ");
        yoltipi=input.nextInt();

        System.out.print("lütfen kaç km gideceğinizi yazınız: ");
        mesafe=input.nextInt();

      toplampara= (mesafe)*10;
      if(yas<12)
      {
          toplampara=toplampara-(toplampara*50)/100;
          System.out.print("Yeni ücretiniz: "+toplampara);
      } else if (yas>=12 && yas<=24) {
          toplampara=toplampara-(toplampara*10)/100;
          System.out.print("Yeni ücretiniz: "+toplampara);

      } else if (yas>=65) {
          toplampara=toplampara-(toplampara*50)/100;
          System.out.print("Yeni ücretiniz: "+toplampara);

      } else if (yoltipi==2) {
          toplampara=toplampara-(toplampara*20)/100;
          System.out.print("Yeni ücretiniz: "+toplampara);

      }
      else if(yoltipi!=1 && yoltipi!=2)
      {
          System.out.print("Hatalı giriş yaptınız");
      }


    }
}

    
