import java.util.Scanner;

public class main {
  
  public static void main(String[] args) {
       
       
       String userName, password, newPassword, secim;

        Scanner input = new Scanner(System.in);

        System.out.print("Kullanici Adi:");
        userName = input.nextLine();

        System.out.print("Sifre:");
        password = input.nextLine();

        if (userName.equals("patika") && password.equals("java123")) {
            System.out.print("Giris Yaptiniz.");
        } else {
            System.out.println("Bilgiler Yanlis.");
        }

        System.out.println("Sifrenizi Sifirlamak Ister misiniz? ");
        secim = input.nextLine();

        if (secim.equals("evet")) {
            System.out.print("Yeni Sifreyi Giriniz:");
            newPassword = input.nextLine();

            if (newPassword.equals(password)) {
                System.out.print("Sifre Olusturulamadi,lutfen baske sifre giriniz.");
            } else if (newPassword.equals("java123")) {
                System.out.print("Sifre Olusturulamadi,lutfen baske sifre giriniz.");
            } else {
                System.out.print("Sifre Olusturuldu.");
            }
        } else if (secim.equals("hayir")) {
            System.out.println("Sifre Olusturulamadi.");
        } else {
            System.out.print("lutfen tekrar denyin");
        }
    }
}
