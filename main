#include <stdio.h>
#define length 30
#define N 4

 struct{
    char nombre[length];
    char carreras[length];
}facultad[N];

struct{
    char nombre[length];
    int codigo;
    char semestres[];
}carrera[N];

struct{
    char *nombre;
    int codigo;
    char materias[];
}semestre;

struct{
    char *nombre;
    int codigo;
    char paralelos[];
}materia;

struct{
    char *nombre;
    int codigo;
    char alumnos[];
}paralelo;

struct{
    char *nombre;
    double cedula;
    char correo;
}alumnos;

struct{
    double cedula;
    int codigo_paralelo;
    float nota;
}matricula;



void MenuFacultad();
void MenuCarrera();

void leerdatos();

int main (){
    int opc;

    do {
        printf ("\n***** Menu *****\n");
        printf ("1. CRUD Facultad\n");
        printf ("2. CRUD Carrera\n");
        printf ("3. CRUD Semestre\n");
        printf ("4. CRUD Paralelo\n");
        printf ("5. CRUD Alumno\n");
        printf ("6. Matricular\n");
        printf ("7. Asignar nota a estudiante\n");
        printf ("8. Consulta de notas y promedio por codigo de paralelo\n");
        printf ("9. Consulta de notas y promedio por codigo de materia\n");
        printf ("10. Consulta de notas por cedula\n");
        printf ("0. Salir\n");
        printf ("\nSeleccione una opcion: ");
        scanf("%i",&opc);

        switch (opc){
            case 0:
                printf ("\nSaliendo del programa...");
                break;
            case 1:
                printf ("\nCRUD Facultad");
                MenuFacultad();
                break;
            case 2:
                printf ("\nCRUD Carrera");
                MenuCarrera();
                break;
            case 3:
                printf ("\nCRUD Semestre");
                break;
            case 4:
                printf ("\nCRUD Paralelo");
                break;
            case 5:
                printf ("\nCRUD Alumno");
                break;
            case 6:
                printf ("\nMatricular");

                break;
            case 7:
                printf ("\nAsignar Nota a estudiante");
                break;
            case 8:
                printf ("\nConsulta de notas y promedio por codigo de paralelo");
                break;
            case 9:
                printf ("\nConsulta de notas y promedio por codigo de materia");
                break;
            case 10:
                printf ("\nConsulta de nota por cedula");
                break;
        }

    } while (opc != 0);

}

void MenuFacultad(){
    int opc,i,cond;

    do {
        printf ("\n1. Crear nueva facultad");
        printf ("\n2. Ver datos de facultad");
        printf ("\n3. Actualizar datos de facultad");
        printf ("\n4. Volver al menu principal\n");
        printf ("\nSeleccione una opcion: ");
        scanf("%d",&opc);

        switch (opc){
            case 1:
                do{
                    for (i=0;i<N;i++){
                        printf("\nLista de facultades existentes actualmente:\n");
                        for(i=0;i<N;i++){
                            printf("%i. %s \n",i,facultad[i].nombre);
                        }
                        printf("\nIngrese la posicion en la que desea guardar la facultad: ");
                        scanf("%i",&opc);
                        printf("\nIngrese nombre para la facultad: ");
                        scanf("%s",facultad[opc].nombre);
                        printf ("\nLa facultad %s, ha sido creada con exito.",facultad[opc].nombre);
                        printf("\nDesea crear otra facultad? Si=1 / No=0 ");
                        scanf("%i",&cond);

                    }
                 } while (cond != 0);
             
                break;
                
            case 2:
                printf("\nLista de facultades existentes actualmente: \n");
                for(i=0;i<N;i++){
                    printf("%i. %s \n",i,facultad[i].nombre);
                }
                printf ("\nIngrese el numero de la facultad que desea consultar:");
                scanf("%i",&opc);

                printf("Facultad seleccionada:  %s \n",facultad[opc].nombre);
                printf("Carreras de la facultad: %s ");
                printf("\n");

                break;
               

            case 3:
                printf("\nLista de facultades existentes actualmente:\n");
                for(i=0;i<N;i++){
                    printf("%i. %s \n",i,facultad[i].nombre);
                }
                printf ("\nIngrese numero de la facultad que desea actualizar datos: ");
                scanf("%i",&opc);
                printf("Facultad seleccionada:  %s \n",facultad[opc].nombre);
                printf("Ingrese nuevo nombre para la facultad %s: \n",facultad[opc].nombre);
                scanf("%s",facultad[opc].nombre);
                printf("Nuevo nombre de la facultad: %s \n",facultad[opc].nombre);

                break;

            case 4:
                printf ("\nVoliendo al menu principal...\n");
                break;
        }

    } while (opc != 4);

}

void MenuCarrera(){
    int opc,i,cond;

    do {
        printf ("\n1. Crear nueva carrera");
        printf ("\n2. Ver datos de la carrera");
        printf ("\n3. Actualizar datos de la carrera");
        printf ("\n4. Volver al menu principal\n");
        printf ("\nSeleccione una opcion: ");
        scanf("%d",&opc);

        switch (opc){
            case 1:
                do{
                    for (i=0;i<N;i++){
                        printf("\nLista de carreras existentes actualmente:\n");
                        for(i=0;i<N;i++){
                            printf("%i. Codigo: %i | Nombre: %s \n",i,carrera[i].codigo,carrera[i].nombre);
                        }
                        fflush(stdin);
                        printf("\nIngrese la posicion en la que desea guardar la carrera: ");
                        scanf("%i",&opc);
                        printf("\nIngrese nombre para la carrera: ");
                        scanf("%s",carrera[opc].nombre);
                        fflush(stdin);
                        printf ("\nIngrese codigo para la carrera: ");
                        scanf("%i",&carrera[opc].codigo);
                        printf ("\nEl codigo ingresado fue: %i",carrera[opc].codigo);
                        printf ("\nLa carrera %s, ha sido creada con exito.",carrera[opc].nombre);
                        printf("\nDesea crear otra carrera? Si=1 / No=0 ");
                        scanf("%i",&cond);

                    }
                } while (cond != 0);
                break;
          
            case 2:
                printf("\nLista de carreras existentes actualmente: \n");
                for(i=0;i<N;i++){
                    printf("%i. Codigo: %i | Nombre: %s \n",i,carrera[i].codigo,carrera[i].nombre);
                }
                printf ("\nIngrese el numero de la carrera que desea consultar:");
                scanf("%i",&opc);

                printf("Carrera seleccionada:  %s \n",carrera[opc].nombre);
                printf("Codigo de la carrera: %i \n",carrera[opc].codigo);
                printf ("Semestres de la carrera: %i");
                printf("\n");

                break;
               

            case 3:
                printf("\nLista de carreras existentes actualmente: \n");
                for(i=0;i<N;i++){
                    printf("%i. Codigo: %i | Nombre: %s \n",i,carrera[i].codigo,carrera[i].nombre);
                }
                printf ("\nIngrese numero de la carrera que desea actualizar datos: ");
                scanf("%i",&opc);
                printf("Carrera seleccionada:  %s \n",carrera[opc].nombre);
                printf("Codigo de la carrera: %i \n",carrera[opc].codigo);
                printf("Ingrese nuevo nombre para la carrera %s: \n",carrera[opc].nombre);
                scanf("%s",carrera[opc].nombre);
                printf("Nuevo nombre de la carrera: %s \n",carrera[opc].nombre);
                //Desea actualizar el codigo de la carrera? si / no

                break;

            case 4:
                printf ("\nVoliendo al menu principal...\n");
                break;
        }

    } while (opc != 4);

}
