import java.util.Scanner;

public class usodewhile {

    public static void main(String[] args) {


        Scanner n=new Scanner(System.in);
/*
        System.out.println("Tabla de multiplicar\n");
        System.out.println("Ingrese numero para la tabla: ");
        int v1=n.nextInt();
        int v2=0;
        while(v2<13){
            int resultado=v1*v2;
            System.out.println(v1+" x "+v2+" = "+resultado);
            v2++;
        }*/

      /*  System.out.println("Programa de registro de nombres\n");
      String nombre[]=new String[6];
      int edad[]=new int[6];
      int x=0;
        while(x<6){
            System.out.print("Escriba su nombre: ");
            nombre[x]=n.nextLine();
            System.out.print("Ingrese su edad: ");
            edad[x]=n.nextInt();
            n.nextLine();
            x++;

        }
        int y=0;
        while(y<6){
            System.out.println("Su nombre "+y+" es "+nombre[y]+" y su edad es: "+edad[y]);
            y++;
        }

        */

        /*Validar una vocal*/


        System.out.println("Tabla de multiplicar\n");
        System.out.println("Ingrese numero para la tabla (Desde el 1 al 12): ");
        int tabla=n.nextInt();
        
        
                    if (tabla>1 && tabla<=12) {
                        while (tabla >= 1 && tabla <= 12) {
                            int contador = 1;
                                while (contador <= 12) {
                                    int resultado = contador * tabla;
                                    System.out.println(tabla + " x " + contador + " = " + resultado);
                                    contador++;
                                }
                                    System.out.println("Ingrese numero para la tabla: ");
                                     tabla = n.nextInt();
                            if (tabla>12 || tabla<1){
                                System.out.println("Salio del rango");}

                        }
                        }else{
                                System.out.println("Salio del rango");
                        }
    }

}



