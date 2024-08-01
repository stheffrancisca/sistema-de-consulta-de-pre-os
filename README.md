# sistema-de-consulta-de-pre-os
Seu sistema deve:
- Pedir para o usuário o nome de um produto
- Caso o produto exista na lista de produtos, o programa deve retornar o preço do produto como resposta
       - Ex: O produto celular custa R$1500
- Caso o produto não exista na lista de produtos, o programa deve printar uma mensagem para o usuário tentar novamente

- produtos = ["celular", "camera", "fone de ouvido", "monitor"]
precos = [1500, 1000, 800, 2000]
produto_procurado = input("Digite o produto:")
produto_procurado = produto_procurado.lower()
if produto_procurado in produtos:
    indice = produtos.index(produto_procurado)
    preco = precos[indice]
    print(f"Produto: {produto_procurado}, Preço: {preco}")
else:
    print("Produto não encontrado, tente novamente")
