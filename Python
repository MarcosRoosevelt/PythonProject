lista = [[], []]
dic = dict()
inf = dict()
while True:
    dic.clear()
    inf.clear()
    dic['nome'] = str(input('Nome do filme: ')).rstrip().title()
    dic['ano de lanc'] = int(input('Ano de lançamento: '))
    dic['classificação'] = str(input('Classificação: '))
    inf['diretor'] = str(input('Diretor: ')).title().rstrip()
    inf['sinopse'] = str(input('Sinopse do filme: ')).capitalize().rstrip()
    inf['gênero'] = str(input('Gênero do filme: ')).rstrip().title()
    inf['distribuidora'] = str(input('Distribuidora: ')).rstrip().title()

    lista[0].append(dic.copy())
    lista[1].append(inf.copy())

    resp = str(input('Deseja continuar? [S/N] ')).rstrip().upper()[0]
    while resp not in 'SN':
        resp = str(input('Erro! Informe apenas sim[S] ou não[N]: ')).rstrip().upper()[0]
    if resp == 'N':
        break
print(f'-=' * 40)
print(f'cod ', end='')
for i in dic.keys():
    print(f'{i.upper():<30}', end='')
print()
print(f'-=' * 40)
for k, v in enumerate(lista[0]):
    print(f'{k:<3} ', end='')
    for d in v.values():
        print(f'{str(d):<30} ', end='')
    print()
print(f'-=' * 40)

while True:
    opc = int(input('Informe o filme que você ver as informações: '))
    if opc == 999:
        break
    else:
        for i in lista:
            print(i[opc])
