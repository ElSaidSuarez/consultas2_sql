## Ejercicios consulta2.

## 1.Traer el nombre, cedula y salario de un empleado, ordenando los campos de la siguiente manera : Ascendente por nombre y descendente por cedula 

SELECT NOMBRE, CEDULA, SUELDO, FROM, EMPLEADOS WHERE (CIUDAD=`medellin`)ORDER BY NOMBRE;
! [consulta1](img/consulta1.png "Consultas 1")

SELECT NOMBRE, CEDULA, SUELDO, FROM, EMPLEADOS WHERE (CIUDAD=`medellin`)ORDER BY CEDULA DESC;
! [consulta1](img/consulta1-2.png "Consultas 1")

## 2.traer el nombre y salario de los primeros 25 empleados cuyo sueldo es mayor de $600000 ordenandolos en forma ascendente por el numero de cedula

SELECT nombre, sueldo FROM Empleado WHERE (sueldo>600000) ORDER by cedula limit 2;

! [consulta2](img/consulta2.png "Consultas 2")

## 3.mostrar el nombre, id y cedula de los primeros 15 empleados cuyos nombres sean distintos. orden la consulta en forma descendete por cedula

SELECT DISTINCT top 15 nombre,ID,cedula FROM Empleado  ORDER by cedula DESC;

! [consulta3](img/consulta3.png "Consultas 3")

## 4. entregar los 15 primeros empleados  con nombre y cedula cuya ciudad sea BOGOTA. se necesita que todos los encabezados de las columnas tengan los siguientes titulos:
## A. para el campo NOMBRE......... razon social
## B. para el campo CEDULA......... identificacion
## c. ordene la lista en forma descendente por cedula 

SELECT top 15 nombre as "razon social", cedula as "identificacion" FROM empleado WHERE (ciudad = "bogota") order by cedula DESC;

! [consulta4](img/consulta4.png "Consultas 4")

## 5. realizar una consulta que entregue el nombre, identificacion, sueldo, edad, de los empleados cuyos sueldos esten entre $800000 y $1200000 y cuyas edades esten entre los 23 y 30 años

SELECT NOMBRE, CEDULA, SUELDO, EDAD, FROM EMPLEADO, WHERE, (SUELDO BETWEEN 800000 AND 12000000 AND EDAD BETWEEN 23 AND 30)

! [consulta5](img/consulta5.png "Consultas 5")

## 6. Realizar una consulta que muestre nombre, cedula y salario de los empleados cuyo nombre comience por la letra c. ordene esta lista por salario en forma descendente.

SELECT NOMBRE, CEDULA, SUELDO, FROM EMPLEADOS WHERE (NOMBRE LIKE `c%`) ORDER BY SUELDO DESC;

! [consulta5](img/consulta6.png "Consultas 6")