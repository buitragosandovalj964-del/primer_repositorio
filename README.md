# archivo de tipo de markdowon


## titulos de segundo nivel

### titulo de terce nivel

este es un **ejemplo** de un _archivo markdown_.



def alcancia_digital():
    saldo = 0

    while True:
        print(""" BIENVENIDO A TU ALCANCIA DIGITAL
-------------------------
1. AGREGAR SALDO
2. SACAR DINERO
3. VER SALDO
4. SALIR
-------------------------
""")

        opcion = int(input("Elija una opción: "))

        if opcion == 1:
            monto = int(input("Escriba el monto a ingresar: "))
            if monto > 0:
                saldo = saldo + monto
                print("Depósito exitoso. Saldo actual:", saldo)
            else:
                print("Monto inválido")

        elif opcion == 2:
            sacar = int(input("Escriba el monto a retirar: "))
            if sacar <= 0:
                print("Monto inválido")
            elif sacar > saldo:
                print("Saldo insuficiente")
            else:
                saldo = saldo - sacar
                print("Retiro exitoso. Saldo actual:", saldo)

        elif opcion == 3:
            print("Su saldo es:", saldo)

        elif opcion == 4:
            print("Gracias por usar su alcancía digital")
            return

        else:
            print("Opción inválida")

