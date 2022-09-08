# Segurança do Kindelia

Quando eu entrei no mercado de crypto, muito se falava sobre escalabilidade, porem, quanto mais fundo eu adentrava, mais inseguro eu me sentia.

Quase todo dia, me aparecia noticias de hacks e bugs em contrato do tipo:
“Contrato X sofreu um exploit e perdeu N criptomoedas”
e isso continua seguindo.

Nos anos de 2021 até julho de 2022, foram roubados mais de 4 bilhões de dolares em crypto, advindos de problemas com smart contracts e afins.

### Função Kill (Problema 1)
No dia 06 de novembro de 2017, um usuário do github chamado de "devops199" descobriu um bug na rede ethereum, que fazia com que ele pudesse "destruir" contratos multisig que não era de propriedade dele. nesse "acidente" (assim como afirmado por ele), foram perdido mais de 300 milhões de dolares em ETH


### Poly Network exploit (Problema 2)
Porem, essa não foi nem de perto a maior das perdas.
Em agosto de 2021, A Poly network sofreu um exploit em seu contrato proxy em 3 chains diferentes:
Ethereum, Binance Smart Chain (BSC) e Polygon.
Por Poly Network ser um projeto cross-chain, ela possui um contrato protegido que tem o poder de fazer chamadas em outra blockchain. nesse contrato, existe uma função que pode ser chamada e executada por qualquer pessoa para realizar uma transação "cross-chain". se aproveitando de falhas entre diversas funções nesse contrato, o hacker conseguiu ignorar a verificação "onlyOwner" do contrato, permitindo com que ele chamasse uma função que altera chaves publicas.
Nesse exploit, foram roubados mais de 611 milhões de dolares em diversas criptomoedas.


### Qubit Finance bug lógico (Problema 3)
Em outro caso similar, temos a Qubit.
Qubit Finance é também, um projeto cross-chain, que permite colateralização entre chains, no caso, Ethereum x BSC, através de uma função de deposito chamada "QBridge". Em Janeiro de 2022, um usuário se aproveitou de um bug lógico no código da função, que permitiu com que o usuário tivesse acesso a mais de 77,162 qXETH, para usar como colateral em um emprestimo na Qubit.
O atacante usou esses colaterais para pegar "emprestado" cerca de 200 mil BNBs, o que, na época, equivaleria a 80 milhões de dólares.


## Conclusão
E esses são só 3 dos variados roubos que acontecem quase toda semana. De acordo com o site “Web3 Is Going Great” e “rekt.news” de 2020 até a atualidade foram perdidos cerca de 11 bilhões de dolares em cripto. A maioria desses roubos, são frutos de bugs e contratos mal escritos. Mesmo que todos tenham sido auditados, auditores, por limitação humana, são incapazes de provar para todas vertentes de um ataque. No entanto, há uma forma de garantir que a auditagem seja perfeita, com Formal proofs.


## Formal Proofs (Solução)
Provas formais/Provas matemáticas
São demonstrações de que, dados certos axiomas, algum enunciado de interesse é necessariamente verdadeiro. Utiliza como base premissas intrínsecas a um modelo conceitual e um silogismo que, a partir de uma série de operações, chega ao resultado. 

// deixar claro o porque isso é hack-proof 

// Exemplo simples de prova formal

Mas você se pergunta, e por que os programadores não utilizam de formal proofs?
Pelo simples fato de que, realizar formal proofs nas blockchains atuais é muito caro e inviável.
Se para provar formalmente um "hello world" custa 2000 dolares, o custo de uma verificação formal de um codigo de 1400 linhas, como a qBridge da qubit, teria um preço extremamente inviável, que chama diversas funções que não são provadas. 
mas não para a Kindelia
