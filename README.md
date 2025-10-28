# numeros-primos
def _primo(n):
    if n <= 1:
        return False

    divisores = 0
    for i in range(1, n + 1):
        if n % i == 0:
            divisores += 1

    return divisores == 2

for numero in range(1, 101):
    if _primo(numero):
        print(f"{numero} é primo")
    else:
        print(f"{numero} não é primo")
