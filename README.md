
def add(num1, num2):
    return num1 + num2


def subtract(num1, num2):
    return num1 - num2


def multiply(num1,num2):
    return num1 * num2


def divide(num1, num2):
    if num2== 0:
        return "Erro! Divisão por zero."
    return num1 /num2

def calculator():
    print("Selecione a operação:")
    print("1. Adição")
    print("2. Subtração")
    print("3. Multiplicação")
    print("4. Divisão")

    while True:
       
        choice = input("Digite sua escolha (1/2/3/4): ")


        if choice in ('1', '2', '3', '4'):
            try:
                num1 = float(input("Digite o primeiro número: "))
                num2 = float(input("Digite o segundo número: "))
            except ValueError:
                print("Entrada inválida! Por favor, insira um número.")
                continue

            if choice == '1':
                print(f"{num1} + {num2} = {add(num1, num2)}")

            elif choice == '2':
                print(f"{num1} - {num2} = {subtract(num1, num2)}")

            elif choice == '3':
                print(f"{num1} * {num2} = {multiply(num1, num2)}")

            elif choice == '4':
                result = divide(num1, num2)
                print(f"{num1} / {num2} = {result}")

            next_calculation = input("Deseja realizar outra operação? (s/n): ")
            if next_calculation.lower() != 's':
                break
        else:
            print("Opção inválida! Por favor, selecione uma opção válida.")

if __name__ == "__main__":
    calculator()

def add(num1, num2):
    return num1+ num2


def subtract(num1, num2):
    return num1 - num2


def multiply(num1, num2):
    return num1 * num2

def divide(num1, num2):
    if num2 == 0:
        return "Erro! Divisão por zero."
    return num1 / num2

def calculator():
    print("Selecione a operação:")
    print("1. Adição")
    print("2. Subtração")
    print("3. Multiplicação")
    print("4. Divisão")

    while True:
        
        choice = input("Digite sua escolha (1/2/3/4): ")

        
        if choice in ('1', '2', '3', '4'):
            try:
                num1 = float(input("Digite o primeiro número: "))
                num2 = float(input("Digite o segundo número: "))
            except ValueError:
                print("Entrada inválida! Por favor, insira um número.")
                continue

            if choice == '1':
                print(f"{num1} + {num2} = {add(num1, num2)}")

            elif choice == '2':
                print(f"{num1} - {num2} = {subtract(num1, num2)}")

            elif choice == '3':
                print(f"{num1} * {num2} = {multiply(num1, num2)}")

            elif choice == '4':
                result = divide(num1, num2)
                print(f"{num1} / {num2} = {result}")

           
            next_calculation = input("Deseja realizar outra operação? (s/n): ")
            if next_calculation.lower() != 's':
                break
        else:
            print("Opção inválida! Por favor, selecione uma opção válida.")

if __name__ == "__main__":
    calculator()
