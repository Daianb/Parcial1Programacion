# Parcial1Programacion
Estudiante D: Implemente un metodo que

1. Reciba una lista de listas (matriz) donde cada elemento sea un número complejo en formato cadena y lo guarde de alguna manera en un atributo. Un ejemplo de lo que se le puede ingresar es [["2 - 3i,"-i],["4","-5+2i"]]
2. Implemente el metodo _ _ str _ _ para imprimir la matriz
3. Implemente los metodos _ _ mul _ _ y _ _ rmul_ _ para multiplicar matrices entre si teniendo en cuenta que las matrices no son necesariamente conmutativas
4. Implemente la suma de matrices y resta por medio del metodo _ _ add_ _ y _ _ sub_ _

Si se pide que construya una clase que pueda hacer algo, debe implementar un ejemplo de uso en el codigo.

# Desarrollo
- Punto 1. Una matriz que recibe una lista de lista
Como en este proceso y codigo largo no corria el programa, procedi a buscar una solucion, a lo cual haye un metodo mas sencillo y corto y el cual si corria el codigo :D en la parte inicial de definir la matriz. Principalmente use varios ciclos y condicionales, luego con el metodo complex y dos ciclos e in, se pudo acotar la definicion de la matriz a una sola linea y que corriera.
- Punto 2. Implemente el metodo _ _ str _ _ para imprimir la matriz. 
Empece calculando la longitud maxima de cada numero en la matriz, cree una lista de cadenas con un ciclo, uniendo las filas en una sola cadena separadas por un espacio. Usando el metodo .join pude por algo menos estetico dejar el codigo en una linea en vez de 6. Asi que ese deje.
- Punto 3. Implemente los metodos _ _ mul _ _ y _ _ rmul_ _ para multiplicar matrices entre si teniendo en cuenta que las matrices no son necesariamente conmutativas
     - Para la primera parte del punto _ _ mul _ _ Empece con un condicional en el cual filtra que las matrices sean de la misma dimension, tal de que no sea asi en el ValueError aparece el mensaje del porque, cree res que es una matriz que empieza en cero con tantas filas como la primera matriz multiplicada y tantas columnas como la segunda matriz multiplicada, segui con unos ciclos para generar la matriz resultado, recorriendo asi filas y columnas. Para cada elemento de la matriz resultado res, se realiza la suma de los productos de los elementos correspondientes de las matrices originales. Esta operación se realiza para todos los elementos de la matriz resultado.
     - Para la segunda parte del punto _ _ rmul _ _, Uso el termino isinstance que me permite verificar que la matriz va a ser multiplicada por un numero entero, flotante u complejo, sin tener que usar condicionales para tal. Por ejemplo si el usuario ingresa una letra, aparecera un Error con el mensaje seleccionado de que eso no es posible su solicitud. Luego creo una nueva matriz compleja llamada res, que es una copia de la matriz original self. Esto es para asegurarnos de que la operación de multiplicación no modifique la matriz original. Finalmente con ciclos realizo la multiplicacion del termino otra por cada elemento de la matriz, se guarda en res y se retorna.
- Punto 4. Implemente la suma de matrices y resta por medio del metodo _ _ add_ _ y _ _ sub_ _
     - Para la primera parte del punto, _ _ add _ _ Compruebo que las matrices tengan las mismas dimensiones . Si no es así, se genera una excepción ValueError con el mensaje y su respectiva razon, creo nuevamente como arriba una nueva matriz, compleja llamada res, que es una copia de la matriz original self. Esto es para asegurarnos de que la operación de multiplicación no modifique la matriz original.Para el final, con ciclos realizo la suma de las matrices de cada termino que haya en ij: 00, 01, etc.. 
     - Para la segunda parte del punto, _ _ sub _ _ Igualmente que en la definicion de la suma pero esta vez para la resta, para iniciar compruebo que las matrices tengan la misma dimension, creo una matriz res que es una copia de la original, para que no quede con ningun termino usado anteriormente y con ciclos se genera la resta de cada termino.
     
- Ejemplo de uso. Creo un ejemplo de uso para que el usuario confirme que el programa funciona correctamente con dos matrices de 2x2 y otra de 3x3, se escriben las operaciones y se imprimen.


    
