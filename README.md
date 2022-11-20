# Udemy-java
package generartabla;

/**
 *
 * @author GERMAN
 */
import java.util.Scanner;
public class GenerarTabla {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer = new Scanner(System.in);
        
        System.out.println("Ingrese un numero entero: ");
         int n= leer.nextInt();
         
         int c= 0;
         
         while(c <= 10){
             System.out.printf("%d x %d= %d \n", n,c,(n*c));
             c++;
    }
    }
    
}


///package dias;

/**
 *
 * @author GERMAN
 */
import java.util.Scanner;

public class Dias {
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer = new Scanner(System.in);
        
        System.out.println("Ingrese un numero de la semana: ");
        int dia = leer.nextInt();
        String nombreDia = null;
        
        switch (dia){
            case 1:
                nombreDia= "Domoingo";
                break;
                 case 2:
                nombreDia= "Lunes";
                break;
                 case 3:
                nombreDia= "Martes";
                break;
                 case 4:
                nombreDia= "Miercoles";
                break;
                 case 5:
                nombreDia= "Jueves";
                break;
                  case 6:
                nombreDia= "Viernes";
                break;
                 case 7:
                nombreDia= "Sabado";
                break;
                 default:
                     System.out.println("Il numero ingresado es incorrecto");
        }
        System.out.println("El dia es: "+ nombreDia);
    }
    
}


///package espar;

/**
 *
 * @author GERMAN
 */
import java.util.Scanner;

public class EsPar {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer= new Scanner(System.in);
        
        System.out.print("Ingrese un numero: ");
        int n= leer.nextInt();
        
        if(n % 2 == 0){
            System.out.println("ES PAR");
        }else{
            System.out.println("ES IMPAR");
        }
    }
    
}

///package precioventa;

/**
 *
 * @author GERMAN
 */
import java.util.Scanner;

public class PrecioVenta {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer = new Scanner(System.in);
        
        System.out.print("Ingrese valor de venta: ");
        double vv = leer.nextDouble();
        //IGV 19%, pv= precio de venta, vv = valor de venta
        double igv = vv * 0.19;
        double pv = vv + igv;
        
        System.out.println("Valor de venta: "+ vv);
        System.out.println("IGV: "+ igv);
        System.out.println("Precio de venta: "+ pv);
        
        
    }
    
}

///
package main.java;

/**
 *
 * @author GERMAN
 */
import java.util.Scanner;
public class MainJava {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer = new Scanner(System.in);
        
        System.out.println("Ingrese su nombre");
        String nombre= leer.nextLine();
        
        System.out.println("Ingrese su Edad: ");
        int edad= leer.nextInt();
        
        System.out.println("Ingrese un caracter");
        char C= leer.next().charAt(0);
        
         System.out.printf("Nombre: %s Edad: %d \n, ", nombre, edad);
       
        System.out.println("Nombre: "+ nombre);
        System.out.println("Edad: "+ edad);
        System.out.println("Caracter: "+ C);
        //para sacar el slash contraio: \ alt+92, \t= espacio tabulado 
        System.out.println("\\");
    }
    
}

////
package buclewhile;

/**
 *
 * @author GERMAN
 */
public class BucleWhile {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        
        int c=0;        
       /* while(true){
            System.out.println("No me detendré");
        }//bucle infinito*/
       while(c <= 10){
            System.out.println("El valor de c es: "+c);
            c++;        
    }  
    }
}

///
package sumar;

/**
 *
 * @author GERMAN
 */
import java.util.Scanner;

public class Sumar {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer= new Scanner(System.in);
        
        System.out.print("Ingrese numero 01: ");
        var n1 = leer.nextInt();
         
       System.out.print("Ingrese numero 02: ");
       var n2 = leer.nextInt();
       
       var r= n1 + n2;
       
        System.out.printf("La suma %d + %d = %d \n", n1,n2,r);
    }
    
}

