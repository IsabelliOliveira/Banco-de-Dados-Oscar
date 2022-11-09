<h1 align="center"> E o Oscar vai para... ? :trophy: </h1>

<p>Muito bem, Pessoal... <br>Hoje vamos trabalhar com o Oscar.<br>A ideia de premiar ou ser premiado é para reconhecer:<br>- Reconhecer uma qualidade<br>- Reconhecer um atributo<br>- Reconhecer o esforço... <br>Reconhecer sempre.<br>Nem todos os prêmios são merecidos e nem todos que merecem ganham.<br>Então vale mesmo a pena, premiar?</p>

<h3 :memo:>Aqui vai uma ajudinha:<br>Nesse exercício vamos usar alguns comandos bem básicos como</h3>

>SELECT COUNT(*) FROM tabela_exemplo WHERE coluna_exemplo = "Novo Valor";<br>SELECT * FROM tabela_exemplo WHERE coluna_exemplo = "Novo Valor"  AND coluna_exemplo2 = "Outro Valor";<br>SELECT * FROM tabela_exemplo WHERE coluna_exemplo LIKE 'eda';<br>UPDATE tabela_exemplo SET coluna_exemplo = "Novo Valor" WHERE id = 1;<br>INSERT INTO tabela_exemplo (coluna_1, coluna_2) VALUES ("VALOR 1", "VALOR 2");

<h3> :memo:Quantas vezes Natalie Portman foi indicada ao Oscar?</h3>

>:white_check_mark: Natalie Portman foi indicada 3. 
>
> SELECT * FROM oscar WHERE name LIKE "Natalie Portman"

<h3> :memo:Quantos Oscars Natalie Portman ganhou?</h3>

>:white_check_mark:Natalie Portman ganhou 1 vez.
>
>SELECT * FROM oscar WHERE name LIKE "Natalie Portman"


<h3>:memo:Amy Adams já ganhou algum Oscar?</h3>

> :white_check_mark:Amy Adams não ganhou Oscar.
> 
>SELECT * FROM oscar WHERE name LIKE "Amy Adams";


<h3>:memo:Alguém já ganhou um Oscar e tem o seu primeiro nome?</h3>
<br>

>:radioactive:

<h3>:memo:Toy Story 3 ganhou um Oscar em quais anos?</h3>

> :white_check_mark:O filme Toy Story 3 ganhou 2 vezes no mesmo ano 2011.
>
> SELECT * FROM oscar WHERE film LIKE "Toy Story 3";


<h3>:memo:Quem tem mais Oscars: a categoria "Melhor Ator" ou "Melhor Filme"?</h3>
<br>
<h3>:memo:O primeiro Oscar para melhor Atriz foi para quem? Em que ano?</h3>
<br>
<h3>:memo:Na categoria Winner, altere todos os valores com "True" para 1 e todos os valores "False" para 0.</h3>
<br>
<h3>:memo:Em qual edição do Oscar "Crash" ganhou o prêmio?</h3>
<br>
<h3>:memo:Que filme merecia ganhar um Oscar e não ganhou?</h3>
<br>
<h3>:memo:Bom... dê um Oscar para esse filme, então</h3>
<br>
<h3>:memo:O filme Central do Brasil aparece no Oscar?</h3>
<br>
<h3>:memo:Aliás... Qual sua opinião sobre central do Brasil</h3>
<br>
<h3>:memo:Inclua no banco 7 filmes que nunca nem foram nomeados ao Oscar, mas que na sua opinião, merecem.</h3>
<br>
<h3>:memo:Crie uma nova categoria de premiação. Qualquer prêmio que você queira dar. Agora vamos dar esses prêmios aos filmes que você cadastrou na questão acima.</h3>
<br>
<h3>:memo:Qual foi o primeiro ano a ter um prêmio do Oscar?</h3>
<br>
<h3>:memo:Pensando no ano em que você nasceu: Qual foi o Oscar de melhor filme, Melhor Atriz e Melhor Diretor?</h3>
<br>
<h3>:memo:Agora procure 7 atrizes que não sejam americanas, europeias ou brasileiras.  Vamos cadastrá-los no nosso banco, mas eles ainda não ganharam o Oscar. Só foram nomeados.</h3>
<br>
<h3>:memo:Agora vamos falar da sua vida. Me diga o nome de uma pessoa que você admira e o que ela fez na sua vida. Agora me diz: Quê prêmio essa pessoa merece?</h3>
<br>
<h3>:memo:Utilizando o comando 'Alter Table', troque os tipos dos dados da coluna/campo "Winner" para Bit.</h3>

