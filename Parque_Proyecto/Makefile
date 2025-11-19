############################################################
# Pontificia Universidad Javeriana
# Autor: Danna Gabriela Rojas & María Fernanda Velandia 
# Materia: Sistemas Operativos
# Tema: Proyecto Parque de Berlín
# Fichero: Automatización de Compilación del Sistema
############################################################

GCC = gcc
# -Wall y -Wextra muestran advertencias útiles
# -pthread permite utilizar hilos POSIX
# -g incluye información de depuración
FLAGS = -Wall -Wextra -pthread -g

PROGRAMAS = controlador agente

# Se añaden las carpetas: Sistema, Controlador_de_Reserva y Agente_de_Reserva
INCLUDES = -ISistema -IControlador_de_Reserva -IAgente_de_Reserva

controlador:
	$(GCC) $(INCLUDES) $(FLAGS) \
	Sistema/Sistema.c \
	Controlador_de_Reserva/Controlador.c \
	Controlador_de_Reserva/mainControlador.c \
	-o $@


agente:
	$(GCC) $(INCLUDES) $(FLAGS) \
	Sistema/Sistema.c \
	Agente_de_Reserva/Agente.c \
	Agente_de_Reserva/mainAgente.c \
	-o $@


clean:
	$(RM) $(PROGRAMAS)
