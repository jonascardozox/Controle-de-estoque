# Controle de estoque
Esse projeto consiste na criação de um sistema de controle de estoque onde será possivel:

- Adicionar item;
- Remover item;
- Contolar quantidade de entrada e saída;
- Buscar item;
- exibir lista de item.

<t>após a primeira versão, pedi a IA para analizar sem me enviar o código pronto, e ela me retornou os seguintes pontos:</t>

Para deixar o programa 100% funcional e sem bugs, faltam as seguintes correções e implementações:

Adicionar o item à lista dentro da função adicionar_item: A função apenas valida os dados, mas não insere o dicionário {'nome': nome, 'quantidade': quantidade, 'preço': preço} na lista inventario. A inserção está sendo feita incorretamente dentro do menu().

Verificar duplicidade ao adicionar: O sistema permite cadastrar dois itens com o mesmo nome em vez de apenas somar a quantidade do item existente.

Tratar exceções de digitação no menu(): Se o usuário digitar letras nas opções que pedem número (como quantidade ou preço), o programa quebra com um erro do tipo ValueError.

Tratar a busca por maiúsculas/minúsculas: O programa compara strings de forma exata (diferencia "Caneta" de "caneta"). O ideal é usar .lower() ou .strip() ao comparar nomes.

Ajustar a exibição do produto: O programa imprime o dicionário nativo (ex: {'nome': 'Lápis', ...}). Falta formatar a saída para o usuário ler de forma amigável.

o projeto será desenvolvido com intuito treinar aplicações em Python e também para portifólio.