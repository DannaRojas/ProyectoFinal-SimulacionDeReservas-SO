# Sistema de Reservas para el Parque Berlín

En la realización de este proyecto para la materia de Sistemas Operativos se realizo un programa encargado de realizar reservas teniendo en cuenta la hora, aforo. En caso de no cumplir con lo necesario se mueve la reserva o se niega, todo eso según las condiciones de reserva.

## Modo de uso
1. Abrir dos terminales desde nuestra carpeta de proyecto
2. En la primera terminal ingresar make controlador
3. Ingresar ./controlador -i horaIni -f horaFin -s segHora -t total -p pipeRecibe
4. En la segunda terminal ingresar make agente
5. Ingresar ./agente -s nombreAgente -a nombreArchivo -p pipeRecibe

## Archivo con solicitudes
- El archivo debe ser .csv
- Debe contener familia, hora, numPersonas
- En este proyecto se tiene 6 pruebas.csv

## Anotaciones
Recuerde hacer make clean si llega a salir que ya se encuentra en update el controlador o el agente

### Integrantes 
- Danna Gabriela Rojas Bernal
- María Fernanda Velandia Gracia
