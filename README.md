# inveter_strings

def inverter_string(original):
    caracteres = list(original)

    i, j = 0, len(caracteres) - 1

    while i < j:
        # Troca os caracteres nas posições i e j
        caracteres[i], caracteres[j] = caracteres[j], caracteres[i]

        # Move os índices para o próximo par de caracteres
        i += 1
        j -= 1

    invertida = ''.join(caracteres)

    return invertida

# Exemplo de uso
string_original = "Hello, World!"
string_invertida = inverter_string(string_original)

print(f"String original: {string_original}")
print(f"String invertida: {string_invertida}")
