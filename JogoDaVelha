tabela = {'7': ' ', '8': ' ', '9': ' ',
            '4': ' ', '5': ' ', '6': ' ',
            '1': ' ', '2': ' ', '3': ' '}
chave_tabela = []
for chave in tabela:
    chave_tabela.append(chave)
def desenhartabela(local):
    print(local['7'] + '|' + local['8'] + '|' + local['9'])
    print('-+-+-')
    print(local['4'] + '|' + local['5'] + '|' + local['6'])
    print('-+-+-')
    print(local['1'] + '|' + local['2'] + '|' + local['3'])
def jogo():
    vez = 'X'
    contar = 0

    for i in range(10):
        desenhartabela(tabela)
        print("É a vez de " + vez + ". Digite o lugar?")

        mover = input()

        if tabela[mover] == ' ':
            tabela[mover] = vez
            contar += 1
        else:
            print("Esse lugar já está cheio.\nDigite o lugar?")
            continue
        if contar >= 5:
            if tabela['7'] == tabela['8'] == tabela['9'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['4'] == tabela['5'] == tabela['6'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['1'] == tabela['2'] == tabela['3'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['1'] == tabela['4'] == tabela['7'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['2'] == tabela['5'] == tabela['8'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['3'] == tabela['6'] == tabela['9'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['7'] == tabela['5'] == tabela['3'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
            elif tabela['1'] == tabela['5'] == tabela['9'] != ' ':
                desenhartabela(tabela)
                print("\nFim do Jogo.\n")
                print(" **** " + vez + " venceu. ****")
                break
        if vez == 'X':
            vez = 'O'
        else:
            vez = 'X'
    pergunta = input("Deseja jogar outra vez?(y/n)")
    if pergunta == "y" or pergunta == "Y":
        for chave in chave_tabela:
            tabela[chave] = " "
        jogo()
if __name__ == "__main__":
    jogo()
