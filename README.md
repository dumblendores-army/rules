# RULES

## Nomenclatura 

Nombres de los repos: **asignatura_practicatema_numeroejercicio**

> sotr_p3_ejer2

## Nombres Claves

Posibles nombres claves y sus usos dentro de los codigos:

* **OJO**: Para indicar que hay que tener cuidado con algo, con su pequeña explicacion.
```
// OJO Esto hace falta, sino nos sale en el terminal la palabra temporizador y se cierra el programa
	pthread_sigmask(SIG_BLOCK,&set,NULL);
```

* **CLAVE**: Un bloque de codigo que puede ser clave para algo, si es una funcion se explica como en javadoc, sino, indicar el comienzo y fin del bloque clave. Ejemplo:
```
/* 
*	CLAVE
*	
*  	Funcion para hacer una espera activa
*
*  	@param tiempo tiempo en segundos que queremos que espere la funcion
*/
void espera_activa( int tiempo) {

	time_t t;

	//Bucle de espera 
    t = time(0) + tiempo;
    while(time(0) < t);
}
```

* **OTRO**: Para hacer alguna aclaracion no muy relevante. Ejemplo:
```
// OTRO variables para mi forma de hacer el ejercicio
	uint8_t ciclo = 0x00;
	uint8_t mask = 0x01;
```
