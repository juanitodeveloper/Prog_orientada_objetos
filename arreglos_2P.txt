import java.util.Scanner;

public class arregloclase {

    public static void main(String[] args) {
      /*  Scanner tabla=new Scanner(System.in);
        System.out.print("Ingrese numero de tabla: ");
        int ntabla=tabla.nextInt();

        for(int x=0; x<13; x++){
            int dato=ntabla*x;
            System.out.println(ntabla+" x "+x+" = "+dato);
        } */

        String nombre[]=new String[6];
        int edad[]=new int[6];
        Scanner entrada=new Scanner(System.in);

        for(int x=1; x<7; x++) {
            System.out.println("Escriba su nombre: ");
            nombre[x] = entrada.nextLine();


            System.out.println("Ingrese su edad: ");
            edad[x] = entrada.nextInt();
            entrada.nextLine();



        }

        for(int y=0; y<6; y++) {
            System.out.println("Su nombre "+y+" es "+nombre[y]+" y su edad es "+edad[y]);
        }






    }


}
