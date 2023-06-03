# Mis proyectos en Phyton

#cimc.py es un código que nos permite calcular el índice de masa corporal

#A continución se presenta la calculadora de IMC

# Verificamos que la cantidad de perosnas sea mayor a 0

while personas > 0:

# En las siguientes líneas le pedimos al usuario que ingrese sus datos
    nombre = input("Su nombre por favor: ")
    apellido_paterno = input("Su apellido paterno por favor: ")
    apellido_materno = input("Su apellido materno por favor: ")
    edad = int(input("Su edad por favor: "))
    estatura = float(input("Su estatura en metros por favor: "))
    peso = float(input("Su peso en kilogramos por favor: "))

# Las siguientes líneas nos ayudarán a identificar si el usuario es menor o mayor de edad
    if (edad < 18):
        print("Eres menor de edad")
    else:
        print("Eres mayor de edad")

#Las siguientes líneas harán el cálculo e impresión del IMC

    IMC = peso / estatura**2
    print("IMC: " + str(IMC))

# Hacemos las distintas validaciones
    if IMC >= 0 and IMC <= 15.99:
      print("Delgadez severa")
    elif IMC >= 16.00 and IMC <= 16.99:
      print("Delgadez moderada")
    elif IMC >= 17.00 and IMC <= 18.49:
      print("Delgadez leve")
    elif IMC >=18.50 and IMC <= 24.99:
      print("Normal")
    elif IMC >= 25.00 and IMC <=29.99:
      print("Sobrepeso")
    elif IMC >= 30.00 and IMC <= 34.99:
      print("Obesidad leve")
    elif IMC >= 35.00 and IMC <= 39.99:
      print("Obesidad media")
    elif IMC >= 40.00:
      print("Obesidad morbida")

#Hacemos lo siguiente para cerrar el ciclo while:

    personas = personas - 1
    
    
# Este proyecto fue realizado gracias al apoyo de UCAMP
