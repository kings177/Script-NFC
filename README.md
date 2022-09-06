# Segurança do Kindelia

Quando eu entrei no mercado de crypto, muito se falava sobre escalabilidade, porem, quanto mais fundo eu adentrava, mais inseguro eu me sentia.

Quase todo dia, me aparecia noticias de hacks e bugs em contrato do tipo:
“Contrato X sofreu um exploit e perdeu N criptomoedas”
e isso continua seguindo.

Nos anos de 2021 até julho de 2022, foram roubados mais de 4 bilhões de dolares em crypto, advindos de problemas com smart contracts e afins. 
  * No dia 06 de novembro de 2017, um usuário do github chamado de "devops199" descobriu um bug na rede ethereum, que fazia com que ele pudesse "destruir" contratos multisig que não era de propriedade dele. nesse "acidente" (assim como afirmado por ele), foram perdido mais de 300 milhões de dolares em ETH
    * problema 1 Vulnerabilidade
      * devops199
      
![image](https://user-images.githubusercontent.com/53550620/187800494-1fc3bb47-8971-4d6b-8f2d-674e76a690c1.png)


Porem, esse não foi nem de perto o pior dos problemas.
Em agosto de 2021, A Poly network sofreu um exploit em seu contrato proxy em 3 chains diferentes:
Ethereum,
Binance Smart Chain (BSC),
e Polygon.
Por Poly Network ser um projeto cross-chain, ela possui um contrato protegido que tem o poder de fazer chamadas em outra blockchain. nesse contrato, existe uma função que pode ser chamada e executada por qualquer pessoa para realizar uma transação "cross-chain". se aproveitando de falhas entre diversas funções nesse contrato, o hacker conseguiu ignorar a verificação "onlyOwner" do contrato, permitindo com que ele chamasse uma função que altera chaves publicas.
Nesse exploit, foram roubados mais de 611 milhões de dolares em diversas criptomoedas.
    * problema 2 Humanproof
      * [polynetwork cross-chain contract exploit](https://rekt.news/polynetwork-rekt/)


No entanto, não podemos nos esquecer também, do bug lógico na Qubit Finance.
// TO-DO
  * problema 3 (motivo, quantia)
  o que, quanto, como
    * problema 3 Bug
      * Qubit audited code
      * The DAO
[Qubit rekt](https://rekt.news/qubit-rekt/)


dentre varios outros roubos...

e no total, de acordo com o site “web3isgoinggreat” e “rekt.news” desde 2020 foram perdidos cerca de 11 bilhões de dolares em cripto.
a maioria desses roubos, são frutos de bugs e contratos mal escritos, apesar de todos terem sido auditados, auditores, por limitação humana, é incapaz de provar para todas vertentes de ataque.
só existe uma forma de fazer isso, Formal proofs.
Provas formais/Provas matemamaticas
* Em matemática, uma prova é uma demonstração de que, dados certos axiomas, algum enunciado de interesse é necessariamente verdadeiro. Utiliza como base premissas intrínsecas a um modelo conceitual e um silogismo que, a partir de uma série de operações, chega ao resultado. deixar claro o porque isso é hack-proof 
* Exemplo simples de prova formal
* 
e por que isso não é feito?
fazer formal proofs nas blockchains atuais é muito caro e inviável
se para provar formalmente um hello world custa 2000 dolares, o custo de uma verificação formal de um codigo de 1400 linhas, como a bridge da qubrit, teria um preço extremamente inviável, que chama diversas funções que não são provadas. 
mas não para a Kindelia

# Kindelia
até o dia de hoje, ser roubado era inevitável, com a Kindelia, isso se tornou uma opção.
e então eu decidi criar a Kindelia.


Na Kindelia, esses tipos de roubos seriam resolvidos da seguinte forma:
// TO-DO
