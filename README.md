package javaapplication27;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class JavaApplication27 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      
         Scanner sc = new Scanner(System.in);
         
        int i;
        System.out.println("Input size of array: ");
        int kol=sc.nextInt();
        int[]array=new int[kol];
       
        System.out.println("Input elements of array: ");
        for( i=0; i<kol; i++)
           array[i]=sc.nextInt();  
            int b=0;
        
               boolean f;
               do{
                   f=false;
               for(i=0; i<(kol-1); i++){
                    if(array[i]>array[i+1])
                     {
                     b=array[i];
                      array[i]=array[i+1];
                      array[i+1]=b;
                      f=true;
                     }
               }
               
               }
               while(f);
               System.out.println("Sortirov. massiv - "); 
               for( i=0; i<kol; i++) {                  
                   System.out.print(array[i]+" ");
    }
            }
            }
      
