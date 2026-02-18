# Calculadora-basica
Realice esta calculadora simple como primer proyecto propio! Cualquier cosa a mejorar o que me recomienden para seguir evolucionando sera bienvenido . Gracias

#Calculadora simple en PYTHON
#Este programa realiza operaciones matematicas basicas

print ("=== CALCULADORA SIMPLE ===")
print("Bienvenidos a la calculadora de Matias Gomez")
print("Acontinuaciion te pediremos dos numeros para luego realizar la operacion deseada")

#pedimos al usuario que ingrese dos numeros
numero_1 = float (input("Ingrese el primer numero: "))
numero_2 = float (input("Ingrese el segundo numero: "))

#Mostramos las opciones de operacion
print ("\n Selecciona la operacion: ")
print("1. Sumar(+)")
print("2. Restar (-)")
print("3. Multiplicar(*)")
print("4. Dividir (/)")

#Pedimos que elija una operacion
operacion = input("\n Ingresa el numero de la operacion (1/2/3/4): ")

# Realizamos la operacion segun la eleccion 
if operacion =="1":
    resultado= numero_1 + numero_2
    print (f"\n {numero_1} + {numero_2} = {resultado}")
elif operacion == "2":
    resultado = numero_1 - numero_2
    print(f"\n {numero_1} - {numero_2} = {resultado}")
elif operacion == "3":
    resultado = numero_1 * numero_2 
    print(f"\n {numero_1} * {numero_2} = {resultado}")
elif operacion == "4":
    #Verificamos que no se divide por 0
    if numero_2 != 0:
        resultado = numero_1 / numero_2 
        print(f"\n {numero_1} / {numero_2} = {resultado}")
    else: 
        print("\n ¡ERROR! No se puede dividir por cero. ")

else:
    print("!Opcion invalida! Por favor elige 1,2,3 o 4. ")
    
print(" !Muchas gracias de usar la calculadora de Matias! ")
