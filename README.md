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

//package com.mycompany.forcontinue;

/**
 *
 * @author GERMAN
 */
public class ForContinue {
    public static void main(String[] args) {
        
       for(int i= 0; i<=10; i++){                     
           System.out.println("El valor de i: "+ i);             
           if(i==5){
               System.out.println("saltar a la sgte ejecucion");
               //break
               continue;
           }
           System.out.println("NO ME EJECUTARÉ EN 5");
    }
}
}

///public class Array {
    public static void main(String[] args) {
        
     String nombres [];
     nombres = new String[3];
     
     nombres[0] = "Cecilio";
     nombres[1] = "Jose";
     nombres[2] = "Avila";
     
        System.out.println(nombres[0]);
        nombres[1]="Mario"; //para cambiar datos
        System.out.println(nombres[1]);
        System.out.println(nombres.length);//muestra la longitud del arreglo
       
       int[] array1 = {1,2,3,4,5};
       String[] array2= {"Cecilio","Jose","Avila","Ramos"};
        System.out.println(array1[1]);//devuelve el 2
        
        System.out.println(array2[0]);
        //para llamar todo el arreglo
        String[] nombres2= {"Cecilio ","Jose ","Avila ","Ramos "," Estudiante \n"};
        int i= 0;
        while(i < nombres2.length){
            System.out.print(nombres2[i]);
            i++;
        }
        //ahora lo mismo con for
        String[] nombre= {"Cecilio ","Jose ","Avila ","Ramos "," Estudiante \n"};
        int c=0;
        /*for(int c = 0; c < nombre.length; c++){
            System.out.println(nombre[c]);
        }*/
        //forEtch, hace lo mismo que el for y el while, pero mas corto
        for(String dato : nombre){
            System.out.println(dato);
        }
    }
}


///package com.mycompany.forcontinue;

/**
 *
 * @author GERMAN
 */
public class ForContinue {
    public static void main(String[] args) {
        
       for(int i= 0; i<=10; i++){                     
           System.out.println("El valor de i: "+ i);             
           if(i==5){
               System.out.println("saltar a la sgte ejecucion");
               //break
               continue;
           }
           System.out.println("NO ME EJECUTARÉ EN 5");
    }
}
}

///public class arrayBidimension {
    public static void main(String[] args) {
      //  int[][] x = new int[2][3]; 
        
     /*   x[0][0] = 1;
        x[0][1] = 2;
        x[0][2] = 3;
        
        x[1][0] = 4;
        x[1][1] = 5;
        x[1][2] = 6; */
     //lo sgte es lo mismo que x [][], pero tridimensional ahora
      int[][][] x= {
          {
              {1,2,3},
              {4,5,6},
          },
          {
              {-1,-2,-3},
              {-4,-5,-6},
          },
      };
        /*for(int[] matrizInterna: x ){
        for(int dato: matrizInterna){
            System.out.print(dato );
        }*/ 
        for(int[][] matriz2D: x ){
            for(int []matriz1D: matriz2D){
                for (int dato : matriz1D) {
                    System.out.println(dato);
                }
            }
        /*for(int dato: matrizInterna){
            System.out.print(dato );
        }*/
        }
        
    }
}

///
public class funciones {
    public static void main(String[] args) {
        //saludar();
        sumar(20, 20);
        saludar("YOCELIS AVILA", 11);
        // var nombre "Yocelis";
        //var edad = 11;
    }
    //la funcion static void se ejecuta, pero se debe declarar dentro del Metodo main
    static  void sumar(int a, int b){ //los int a y b son parámetros
    int suma=a+b;
        System.out.println("LA SUMA ES: "+ suma);
    }
    static void saludar( String nombre, int edad){
        System.out.printf("HOLA %s tu edad es %d \n",nombre, edad );//los args van asi: "hola" 
    }
}

//
public class Factorial {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        System.out.println(factorial(5));
    }
    static int factorial(int numero){
        if (numero > 1) {
            numero = numero * factorial( numero - 1);
        }
        return numero;
    }
}

//
public class funcRecursiva {
    public static void main(String[] args) {
        cuentaRegresiva(10);
    }
    static void cuentaRegresiva(int numero){
    numero --;
    
        if (numero > 0) {
            System.out.println(numero);
            cuentaRegresiva(numero);
        }else{
            System.out.println("Llego hasta 0 ");
        }
    }
 
}

////para numeros infinitos(TODAS LAS OPERACIONES Y STRING)
public class varArgs {
    public static void main(String[] args) {
        System.out.println(sumar("CECILIO ",5,5,6,6, 12,120));
    }
    static int sumar(String nombre, int ... numeros){
        System.out.print("LA SUMA DE " + nombre + "ES: ");
        int suma = 0;
        for(int num : numeros){
        suma += num;
        }
    return suma;
    }
}

////para numeros infinitos(TODAS LAS OPERACIONES Y STRING y doubles)
public class varArgs {
    public static void main(String[] args) {
        System.out.println(sumar("CECILIO ",5,5,6,6, 12,120));
       System.out.println(sumar(4.5,5.0,3.9,4.7,4.5,4.1));
    }
    static int sumar(String nombre, int ... numeros){
        System.out.print("LA SUMA DE " + nombre + "ES: ");
        int suma = 0;
        for(int num : numeros){
        suma += num;
        }
    return suma;
    }
     static double sumar(double ... numeros){
        double suma = 0;
        for(double num : numeros){
        suma += num;
        }
    return suma;
}
}

//package clasemath;

public class ClaseMath {
  
    public static void main(String[] args) {
        // TODO code application logic here
        System.out.println(Math.PI);
        System.out.println(Math.E);
        System.out.println(Math.pow(3,3));
        
        System.out.println(Math.random());        
      //  var numerosRandom = Math.random()*101; //devuelve double
      int numerosRandom = (int)(Math.random()*101);//devuelve enteros
        System.out.println(numerosRandom);//devuelve enteros
    }    
}

///
package clasemath;

public class ClaseMath {
  
    public static void main(String[] args) {
        // TODO code application logic here
        System.out.println(Math.PI);
        System.out.println(Math.E);
        System.out.println(Math.pow(3,3));
        
        System.out.println(Math.random());        
      //  var numerosRandom = Math.random()*101; //devuelve double
      int numerosRandom = (int)(Math.random()*101);//devuelve enteros
        System.out.println(numerosRandom);//devuelve enteros
        
         System.out.println(Math.sqrt(64));
         System.out.println(Math.max(15, 25));
         System.out.println(Math.min(15, 25));
         System.out.println(Math.round(25.8777));//redondear numeros
         
         double moneda= (double)Math.round(3.4389 * 100d)/100; //para trabajar con monedas
         System.out.println(moneda);        
         
    }    
}

///


public class ClaseString {
    public static void main(String[] args) {
        String nombre = "Cecilio";
        System.out.println(nombre.charAt(3));
        System.out.println(nombre.length());
        
        for(int i=0; i < nombre.length(); i++){
            System.out.println(nombre.charAt(i));
        }
        System.out.println(nombre.substring(0, 6));
        System.out.println(nombre.toLowerCase());//convierte en minuscula
        System.out.println(nombre.toUpperCase());//convierte en mayusculas
        
        nombre="C E C I L I O";
        System.out.println(nombre.replace(" ", "-"));//reemplaza
        System.out.println(nombre.replace(" ", ""));
        
        System.out.println("Hola".equals("hola"));//false
        System.out.println("Hola".equals("Hola"));//true
        
        //String Builder/ es un constructor
        StringBuilder nuevo= new StringBuilder();
        System.out.println(nuevo);
        
        nuevo.append("HOLA ");
        nuevo.append("MUNDO");
        System.out.println(nuevo.toString());
    }
}

//

package primaridad;

import java.util.Scanner;

public class Primaridad {
   
    public static void main(String[] args) {
        Scanner leer = new Scanner(System.in);
        
        System.out.println("Ingrese un numero: ");
        int numero = leer.nextInt();
        
        if (esPrimo(numero)) {
            System.out.println("============");
            System.out.println("Es numero primo");            
            System.out.println("============");
        }else{            
            System.out.println("============");
            System.out.println("No es un numero primo");            
            System.out.println("============");
        }
    }
    static boolean esPrimo(int numero){
    int contador= 0;
    
    int[] numeros = new int[numero];
    for(int i=0; i<numeros.length; i++){
    numeros[i]= i+1;
    }
    for(int i: numeros){
        if(i == 1 || i == numero){
        continue;
        }
        if(numero % i == 0){
        contador++;
        }
    }
    return contador == 0;
    }
}

///
package espalindromo;

import java.util.Scanner;

public class Espalindromo {
   
    public static void main(String[] args) {
        Scanner leer = new Scanner(System.in);
        System.out.println("Ingrese una palabra: ");
        
        String cadena = leer.nextLine();
        
        if (esPalindromo(cadena)) {
            System.out.println("==============");
            System.out.println("Es palindromo");
            System.out.println("===============");
        }else{
             System.out.println("===============");
            System.out.println("No es palindromo");
            System.out.println("=================");
        }
    }
    static boolean esPalindromo(String cadena){
        
        cadena = cadena.replace(" ", "");
        cadena = cadena.toLowerCase();
        
        StringBuilder cadenaInvertida = new StringBuilder();
        
        for(int i = cadena.length()-1; i >= 0; i--){
            cadenaInvertida.append(cadena.charAt(i));
        }
    return cadena.equals(cadenaInvertida.toString());
    }
}

///
package generarpassword;

public class GenerarPassword {
    
    public static void main(String[] args) {
        System.out.println(generaContrasena());
    }
    static String generaContrasena(){
    char[] mayusculas = {'A','B','C','D','E','F','G'};
    char[] minusculas = {'a','b','c','d','e','f','g'};
    char[] numeros = {'1','2','3','4','5','6','7','8','9','0'};
    
    StringBuilder caracteres = new StringBuilder();
    caracteres.append(mayusculas);
    caracteres.append(minusculas);
    caracteres.append(numeros);
    
    StringBuilder contrasena = new StringBuilder();
    
    for(int i=0; i<= 15; i++){
    int cantidadCaracteres = caracteres.length();
    int numeroRandom = (int)(Math.random()*cantidadCaracteres);
    
    contrasena.append((caracteres.toString()).charAt(numeroRandom));
    }
    
    return contrasena.toString();
    }
}

///
package conversor;

import java.util.Scanner;

public class Conversor {

    public static void main(String[] args) {
        while(true){
            System.out.println("CONVERSOR DE MONEDAS");
            System.out.println("1 - Soles peruanos a dolares\n"
                    +"2 - Pesos Mexicanos a dolares \n"
                    +"3 - Pesos Colombianos a dolares\n"
                    +"4 - Salir" );
            System.out.println("INGRESE UNA OPCION: ");
            
            Scanner leer = new Scanner(System.in);
            char opcion = leer.next().charAt(0);
        }
    }
    static void convertir(double valorDolar, String pais){
        Scanner leer= new Scanner(System.in);
        System.out.printf("Ingrese la cantidad de %s : ", pais);
        double cantidadMoneda = leer.nextDouble();
        
        double dolares = cantidadMoneda / valorDolar;
        dolares = (double) Math.round(dolares * 100d)/100;
        
        System.out.println("------------------------------");
        System.out.println("|   Tienes &"+dolares+"Dolares   |");
        System.out.println("------------------------------");
    }
    
}

////
package conversor;

import java.util.Scanner;

public class Conversor {

    public static void main(String[] args) {
        
        EXTERNA:
        while(true){
            System.out.println("CONVERSOR DE MONEDAS");
            System.out.println("1 - Soles peruanos a dolares\n"
                    +"2 - Pesos Mexicanos a dolares \n"
                    +"3 - Pesos Colombianos a dolares\n"
                    +"4 - Salir" );
            System.out.println("INGRESE UNA OPCION: ");
            
            Scanner leer = new Scanner(System.in);
            char opcion = leer.next().charAt(0);
            
            switch (opcion) {
                case '1':
                    convertir(3.58, "Soles Peruanos");
                    break;
                    case '2':
                    convertir(22.15, "Pesos Mexicanos");
                    break;
                    case '3':
                    convertir(3851.90, "Pesos Colombianos");
                    break;
                case '4':
                    System.out.println("CERRANDO PROGRAMA");
                    break EXTERNA;
                    
                    default:
                        System.out.println("OPCION INCORRECTA");
                        break;
            }            
        }
    }
    static void convertir(double valorDolar, String pais){
        Scanner leer= new Scanner(System.in);
        System.out.printf("Ingrese la cantidad de %s : ", pais);
        double cantidadMoneda = leer.nextDouble();
        
        double dolares = cantidadMoneda / valorDolar;
        dolares = (double) Math.round(dolares * 100d)/100;
        
        System.out.println("------------------------------");
        System.out.println("|   Tienes &"+dolares+" Dolares   |");
        System.out.println("------------------------------");
    }
    
}

///
package juego;

import java.util.Scanner;

public class Juego {

    public static void main(String[] args) {
        // TODO code application logic here
        jugar(5);
    }
    static void jugar(int vidas){
    int numeroRandom = (int)(Math.random()*101);
    int numeroElegido= -1;
    
        Scanner leer = new Scanner(System.in);
        
        while (numeroElegido != numeroRandom){            
            System.out.print("Ingrese un numero entre 1 y 100: ");
            numeroElegido = leer.nextInt();
            
            if (numeroRandom < numeroElegido) {
                System.out.println("El numero es mas pequeño");
                vidas--;
            }else if (numeroRandom > numeroElegido) {
                System.out.println("El numero es mas grande");
                vidas--;
            }
            if (vidas == 0){
                System.out.println("------------------");
                System.out.println("|   GAME OVER    |");
                System.out.println("------------------");
            }
            System.out.println("----------------------");
            System.out.printf("|  Te quedan %d vidas  |\n", vidas);
            System.out.println("-----------------------");
        }
        if (numeroElegido == numeroRandom) {
            System.out.println("--------------------------");
            System.out.println("|   FELICIDADES GANASTE   |");
            System.out.println("--------------------------");
        }
    }    
}

////
package juego;
//para generar un ejecutable JAR. Al lado de Projects Clic en Files, buscamos el proyecto
// Le damos clic derecho y clic properties, Clic en Compiling y marcamos todas las casillas.
//Luego packaging y selecionamos las 3 primeras casillas
//Luego en Run y marcamos ok.
//Luego, en Clean and Build
//Ya lo podemos compartir y ejecutar en cualquier lugar.
// en mi cdm (simbolo del sistema)
// esta es la ruta en mi pc: C:\Users\GERMAN\OneDrive\Escritorio\juego-java
//java -jar Juego.jar


import java.util.Scanner;

public class Juego {

    public static void main(String[] args) {
        //jugar(5);
        
        //complemento/subiendo complejidad del juego
        OUTER:
        while (true) {            
            System.out.println("JUEGO ADIVINA EL NUMERO \n");
            System.out.println("1 - Nivel Facil \n"
            +"2 - Nivel Intermedio \n"
            + "3 - Nivel Dificil \n"
            +"4 - Salir ");
            
        Scanner leer = new Scanner(System.in);
            System.out.print("INGRESE UNA OPCION: ");
            int opcion = leer.nextInt();
            
            switch (opcion) {
                case 1:
                    jugar(10);
                    break;
                case 2:
                    jugar(7);
                    break;
                case 3:
                    jugar(5);
                    break;
                case 4:
                    System.out.println("CERRANDO PROGRAMA");
                    break OUTER;
                default:
                    System.out.println("OPCION INCORRECTA");
            }
        }
    }
    static void jugar(int vidas){
    int numeroRandom = (int)(Math.random()*101);
    int numeroElegido= -1;
    
        Scanner leer = new Scanner(System.in);
        
        while (numeroElegido != numeroRandom){            
            System.out.print("Ingrese un numero entre 1 y 100: \n");
            numeroElegido = leer.nextInt();
            
            if (numeroRandom < numeroElegido) {
                System.out.println("El numero es mas pequeño \n");
                vidas--;
            }else if (numeroRandom > numeroElegido) {
                System.out.println("El numero es mas grande \n");
                vidas--;
            }
            if (vidas == 0){
                System.out.println("------------------");
                System.out.println("|   GAME OVER    |");
                System.out.println("------------------");
                break;
            }
            System.out.println("----------------------");
            System.out.printf("|  Te quedan %d vidas  |\n", vidas);
            System.out.println("-----------------------");
        }
        if (numeroElegido == numeroRandom) {
            System.out.println("--------------------------");
            System.out.println("|   FELICIDADES GANASTE   |");
            System.out.println("--------------------------");
        }
    }    
}

//// POO Y SUS CLASES

package poo1;

public class POO1 {

    public static void main(String[] args) {
        // TODO code application logic here
        persona persona1;
        persona1 = new persona();
        
        persona1.Nombre = "CECILIO";
        persona1.Edad = 35;
        
        persona1.mostrarDatos();
        
           persona persona2;
        persona2 = new persona();
        
        persona2.Nombre = "JOSE MIGUEL";
        persona2.Edad = 40;
        
        persona2.mostrarDatos();
    }
    
}

//
package poo1;

public class persona {
    
    String Nombre;
    int Edad;
    
    void mostrarDatos(){
    
        System.out.println("Nombre: " + Nombre);
        System.out.println("Edad: " + Edad);
    }
}

//////se ha creado un nuevo paquete llamado clases, donde ingresamos persona. esto para menejar
// las importaciones 
//aqui trabajamos las modularizaciones con una clase Main(POO1)
package poo1;
// importamos clases "persona.java"
import clases.persona;
import clases.calculadora;

public class POO1 {

    public static void main(String[] args) {
        // TODO code application logic here
        /*persona persona1 = new persona();
        persona1 = new persona(); 
        persona1.Nombre = "CECILIO";
        persona1.Edad = 35;         
        persona1.mostrarDatos();  
        
        persona persona2 = new persona();
        persona2 = new persona();
        persona2.Nombre = "JOSE MIGUEL";
        persona2.Edad = 40;        
        persona2.mostrarDatos(); */
       
       
        //otra clase:
        System.out.println(calculadora.PI);
        System.out.println(calculadora.sumar(40, 50));
        
        persona persona3 = new persona();
        persona persona4 = new persona("JOSE ");
        
         persona persona5 = new persona();
         persona5.Nombre = "JOSE AVILA";
         persona5.Edad = 37;
         persona5.mostrarDatos();
        
    }
    
}

//
package clases;

public class persona {
    
    public String Nombre;
    public int Edad;
    
    public persona(){
        System.out.println("Construyendo el objeto");
    }
    public persona(String nombre){
        System.out.println("Hola " + nombre + "te llamamos desde el constructor");
    }
    
    public void mostrarDatos(){
    
        System.out.println("Nombre: " + Nombre);
        System.out.println("Edad: " + Edad);
    }
}

//
package clases;

public class calculadora {
    public static double PI = 3.152;
    
    public static int sumar(int a, int b){
        return a + b;
    }
}

////
