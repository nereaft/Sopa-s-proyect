Sopa-s-proyect
==============

#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]){

   int opcion, medida;
 
  do{
   system("clear");
   system("figlet sopa de letras");
   printf("\n\n\t 1.Crear nuevo"
	       "\t 2.Cargar sopa"
               "\t 3.Guardar sopa"
               "\t 4.Salir\n");
   scanf(" %i", &opcion);
   }while(opcion<1 || opcion>4);

   printf("\n\n\t Has elegido ");
   switch(opcion){
     case 1: printf("Crear nuevo.\n");
             break;
     case 2: printf("Cargar sopa.\n");
             break;
     case 3: printf("Guardar sopa.\n");
             break;
     case 4: printf("Salir.\n");
             break;
   }
   if(opcion == 1){
   do{
   printf("\n\n\t Elija un medida:\n"
          "\t\t 1.10x10\n"
          "\t\t 2.15x15\n"
          "\t\t 3.20x20\n"      
         );
   scanf(" %i", &medida);
   }while(medida<1 || medida>3);

   printf("\n\n\t  Has elegido la medida de: ");
   switch(medida){
     case 1: printf("10x10\n");
             break;
     case 2: printf("15x15\n");
             break;
     case 3: printf("20x20\n");
             break;    
   }
}
   if(opcion==2)
      printf("\tCargando...");
   if(opcion==3)
      printf("\tGuardando...");
   if(opcion==4)
      return EXIT_SUCCESS;
   printf("\n\n\n");
     
}
