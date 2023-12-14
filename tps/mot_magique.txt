import java.awt.*;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        final int NB_MAGIQUE = 5;
        int cpt = 0;
        Scanner saisie = new Scanner(System.in);
        int choix;
        do {
            System.out.println("Devinez le nombre magique ");
             choix = saisie.nextInt();
            if (choix != NB_MAGIQUE) {
                System.out.println("mauvais choix");
            }
            cpt++;

        } while ((choix != NB_MAGIQUE) && (choix != 0));
        if(choix == 0){
            System.out.println("Vous avez abondonné la partie, never give up!");
        }else{
            System.out.println("Bravo!! vous avez trouvé le nombre magique après "+cpt+" essais");

        }


    }
}