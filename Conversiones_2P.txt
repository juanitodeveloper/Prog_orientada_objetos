package Clase;

import java.util.Scanner;

public class Funcionesconversionesclase{
    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);


        System.out.println("Programa de conversion\n1)De Masa\n2)De distancia");
        System.out.print("\nSelecciona opcion: ");
        int opcion = entrada.nextInt();


        System.out.print("Ingrese una unidad de medidad: ");
        entrada.nextLine();
        String unidadSigla= entrada.nextLine();

        System.out.print("Ingrese Numero: ");
        double unidadnum= entrada.nextFloat();

        menu(opcion, unidadSigla, unidadnum);
    }
    public static void menu(int opcion, String unidadSigla, double unidadnum) {
    double resultado1;
    String masa, distancia;

        switch (opcion){

            case 1:
                eleccionmasa(unidadSigla,unidadnum);
                resultado1= eleccionmasa(unidadSigla,unidadnum);
                masa=eleccionmasam(unidadSigla);
                System.out.println(resultado1+masa);
               
              
                break;

            case 2:
                elecciondistancia(unidadSigla,unidadnum);
                resultado1= elecciondistancia(unidadSigla,unidadnum);
                distancia=elecciondistanciam(unidadSigla);
                System.out.println(resultado1+distancia);

                break;

            default:
                System.out.println("Esta unidad no esta seleccionada en el parametro de conversion");
                break;

        }

    }

    public static double eleccionmasa(String unidad, double unidaN) {

        double resultado = 0;

        if (unidad.equals("kg") ){
            resultado =unidaN*2.2;
        } else if (unidad.equals("lb") )
            resultado = unidaN / 2.2;



        return resultado;
    }

    public static double elecciondistancia(String unidad, double unidaN) {

        double resultado = 0;

        if (unidad.equals("Km") ){
            resultado =unidaN*1.6;
        } else {if (unidad.equals("mi")) {
            resultado = unidaN / 1.6;
        }
        }

        return resultado;
    }

    public static String eleccionmasam(String unidad) {
            String masa=null;
        if (unidad.equals("kg") ){
           masa=" en Libras(lb)";
        } else {if (unidad.equals("lb")) {
            masa=" en Kilogramos(kg)";
        }
        }
    return masa;
    }

    public static String elecciondistanciam(String unidad) {
        String distancia=null;
        if (unidad.equals("km") ){
           distancia=" en Millas(Mi)";
        } else {if (unidad.equals("mi")) {
           distancia=" en Kilometros(Km)";
        }
        }

    return distancia;
    }
}


