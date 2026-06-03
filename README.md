# code-cesar
def cesar(message, cle):
    alphabet = "abcdefghijklmnopqrstuvwxyz"
    resultat = ""

    for lettre in message:
        position = alphabet.find(lettre)

        if position != -1:
            nouvelle_position = (position + cle) % 26
            resultat = resultat + alphabet[nouvelle_position]
        else:
            resultat = resultat + lettre

    return resultat
