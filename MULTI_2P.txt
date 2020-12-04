
import java.util.Scanner;

public class mutifuncion {

    public static void main(String[] args) {
        Scanner r = new Scanner(System.in);
        String tproductos[] = {"Audifonos", "Computadoras", "Parlantes", "Televisores", "Microondas", "Refrigeradores"};

        int x=0;
        double resultado=0;
        double respuesta;
        
            System.out.println("Sistema de facturacion\n");
            
            System.out.print("Cantidad de productos a llevar: ");
            int cproductos = r.nextInt();
            System.out.println();
            int cantidad[] = new int[cproductos];
            String productos[]=new String[cproductos];
            double precio[] = new double[cproductos];
            String pfproductos[]=new String[cproductos];

            while (x < cproductos) {
                
                System.out.print("Nombre del producto que lleva: ");
                pfproductos[x] = r.nextLine();
                r.nextLine();
                

                    System.out.print("Cantidad del productos que lleva: ");
                    cantidad[x] = r.nextInt();
                    System.out.print("Ingrese el precio: ");
                    precio[x] = r.nextInt();
                    resultado = resultado + (cantidad[x] * precio[x]);
                    
            x++;
            }

            for (int y = 0; y < cproductos; y++) {
                System.out.println("Factura: ");
                System.out.println("Producto " +pfproductos[y]+ " .....Cantidad " + cantidad[y] + " .....Precio " + precio[y]);
            }

            respuesta = resultado;
            System.out.println("Total a pagar: " + respuesta);

            if(respuesta>0){
                double fn=0;
               fn=respuesta-(respuesta*0.15);
                System.out.println("APLICO A UN 15% de descuento ");

                System.out.println("Su total a pagar es de: "+fn);
            }
            
        }
        
    }

  /*   if(band){
             System.out.println("Este producto no se encuentra en el inventario");

             }else{


             }*/
