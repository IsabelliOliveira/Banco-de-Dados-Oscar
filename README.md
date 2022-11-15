<h1 align="center"> E o Oscar vai para... ? :trophy: </h1>

<p>Muito bem, Pessoal... <br>Hoje vamos trabalhar com o Oscar.<br>A ideia de premiar ou ser premiado é para reconhecer:<br>- Reconhecer uma qualidade<br>- Reconhecer um atributo<br>- Reconhecer o esforço... <br>Reconhecer sempre.<br>Nem todos os prêmios são merecidos e nem todos que merecem ganham.<br>Então vale mesmo a pena, premiar?</p>

<h3 :memo:>Aqui vai uma ajudinha:<br>Nesse exercício vamos usar alguns comandos bem básicos como</h3>

>SELECT COUNT(*) FROM tabela_exemplo WHERE coluna_exemplo = "Novo Valor";<br>SELECT * FROM tabela_exemplo WHERE coluna_exemplo = "Novo Valor"  AND coluna_exemplo2 = "Outro Valor";<br>SELECT * FROM tabela_exemplo WHERE coluna_exemplo LIKE 'eda';<br>UPDATE tabela_exemplo SET coluna_exemplo = "Novo Valor" WHERE id = 1;<br>INSERT INTO tabela_exemplo (coluna_1, coluna_2) VALUES ("VALOR 1", "VALOR 2");

<h3> :memo:Quantas vezes Natalie Portman foi indicada ao Oscar?</h3>

> Natalie Portman foi indicada 3. 
>
> :white_check_mark: SELECT * FROM oscar WHERE name LIKE "Natalie Portman"

<h3> :memo:Quantos Oscars Natalie Portman ganhou?</h3>

> Natalie Portman ganhou 1 vez.
>
> :white_check_mark:SELECT * FROM oscar WHERE name LIKE "Natalie Portman"


<h3>:memo:Amy Adams já ganhou algum Oscar?</h3>

> Amy Adams não ganhou Oscar.
> 
> :white_check_mark:SELECT * FROM oscar WHERE name LIKE "Amy Adams";


<h3>:memo:Alguém já ganhou um Oscar e tem o seu primeiro nome?</h3>
<br>

>:radioactive:

<h3>:memo:Toy Story 3 ganhou um Oscar em quais anos?</h3>

> O filme Toy Story 3 ganhou 2 vezes no mesmo ano 2011.
>
> :white_check_mark:SELECT * FROM oscar WHERE film LIKE "Toy Story 3";


<h3>:memo:Quem tem mais Oscars: a categoria "Melhor Ator" ou "Melhor Filme"?</h3>

> A categoria de melhor Filme, com 318.
> 
> :radioactive: SELECT COUNT() FROM oscarWHERE categoryLIKE "Actor"; SELECT COUNT() FROM oscar WHERE category LIKE "CINEMATOGRAPHY";

<h3>:memo:O primeiro Oscar para melhor Atriz foi para quem? Em que ano?</h3>

> O primeiro Oscar foi para Janet Gaynor, no ano de 1928
> 
> :white_check_mark: SELECT * FROM oscar WHERE category LIKE "actress"

<h3>:memo:Na categoria Winner, altere todos os valores com "True" para 1 e todos os valores "False" para 0.</h3>

>:white_check_mark:<br>
>UPDATE oscar <br>
>SET winner= '1' <br>
>WHERE winner='true'; <br>
>
>  UPDATE oscar <br>
>  SET winner= '0' <br>
>  WHERE winner='false';<br>

<h3>:memo:Em qual edição do Oscar "Crash" ganhou o prêmio?</h3>

> :radioactive:
> 
> SELECT year_ceremony FROM oscar WHERE film LIKE '%Crash' AND winner LIKE '%1%';

<h3>:memo:Que filme merecia ganhar um Oscar e não ganhou?</h3>

>:white_check_mark: O Bom dinossauro, não tenho certreza se ele ganhou ou não

<h3>:memo:Bom... dê um Oscar para esse filme, então</h3>

> :radioactive:
> 
> UPDATE oscar SET winner=1 WHERE film LIKE "%divertidamente%" and category LIKE "CINEMATOGRAPHY";

<h3>:memo:O filme Central do Brasil aparece no Oscar?</h3>

> :radioactive: Não
> 
> SELECT * FROM oscar WHERE film LIKE '%Central do Brasil';

<h3>:memo:Aliás... Qual sua opinião sobre central do Brasil</h3>

>:white_check_mark: Nunca assisti ,mas vou colocar na minha lista

<h3>:memo:Inclua no banco 7 filmes que nunca nem foram nomeados ao Oscar, mas que na sua opinião, merecem.</h3>

> :radioactive:
>
> INSERT INTO oscar(id, year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('','2017',NULL,NULL,'MELHOR FILME','Patty Jenkins','MULHER MARAVILHA','1');
> 
> INSERT INTO oscar(id, year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('','2021',NULL,NULL,'MELHOR FILME','Jon Watts','Homem-Aranha: Sem Volta para Casa','1');
> 
> INSERT INTO oscar(id,year_film, year_ceremony, ceremony, category, name, film, winner) VALUES('','2007', '2008','80', 'MELHOR FILME', 'David Fincher','Zodíaco', null);
> 
> INSERT INTO oscar(id, year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('','2021',NULL,NULL,'MELHOR FILME','Sam Raimi','Doutor Estranho no Multiverso da Loucura','0');
> 
> INSERT INTO oscar(id, year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('','2022',NULL,NULL,'MELHOR FILME','Matt Reeves','The Batman','0');
> 
> INSERT INTO oscar(id, year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('','2021',NULL,NULL,'MELHOR FILME','Andy Serkis','Venom: Tempo de Carnificina','0');
> 
>  INSERT INTO oscar(id, year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('','2022',NULL,NULL,'MELHOR FILME','Sam Raimi','Umma','0');


<h3>:memo:Crie uma nova categoria de premiação. Qualquer prêmio que você queira dar. Agora vamos dar esses prêmios aos filmes que você cadastrou na questão acima.</h3>

> :radioactive: ALTER TABLE oscar ADD PRÊMIO varchar(225) UPDATE oscar SET PRÊMIO='BOLO DE CENOURA' WHERE category LIKE '%MELHOR FILME%'

<h3>:memo:Qual foi o primeiro ano a ter um prêmio do Oscar?</h3>

> :radioactive: O primeiro Oscar foi em 1928!
>
> SELECT * FROM oscar WHERE winner;

<h3>:memo:Pensando no ano em que você nasceu: Qual foi o Oscar de melhor filme, Melhor Atriz e Melhor Diretor?</h3>

> :radioactive: Filme - American Beauty
> 
> :radioactive: Atriz - Hilary Swank
> 
> :radioactive: Diretor - Sam Mendes.
>
> SELECT * FROM oscar WHERE year_ceremony LIKE "2000" AND category LIKE "CINEMATOGRAPHY"; <BR>
> SELECT * FROM oscar WHERE year_ceremony LIKE "2000" AND category LIKE "%ACTRESS%";<BR>
> SELECT * FROM oscar WHERE year_ceremony LIKE "2000" AND category LIKE "%DIRECTING%"<BR>

<h3>:memo:Agora procure 7 atrizes que não sejam americanas, europeias ou brasileiras.  Vamos cadastrá-los no nosso banco, mas eles ainda não ganharam o Oscar. Só foram nomeados.</h3>

> :radioactive:
> 
> INSERT INTO oscar (name) VALUES ('Cameron Diaz'), ('Drew Barrymore'), ('Sarah Polley'), ('Emily Blunt'), ('Robin Wright'), ('Charlotte Gainsbourg'), ('Kirsten Dunst');

<h3>:memo:Agora vamos falar da sua vida. Me diga o nome de uma pessoa que você admira e o que ela fez na sua vida. Agora me diz: Quê prêmio essa pessoa merece?</h3>

>

<h3>:memo:Utilizando o comando 'Alter Table', troque os tipos dos dados da coluna/campo "Winner" para Bit.</h3>

> :radioactive:
>
> ALTER TABLE oscar CHANGE winner bit INT(10);


> :white_check_mark: 
> Eduardo Galeano.
“A utopia está lá no horizonte. Me aproximo dois passos, ela se afasta dois passos. Caminho dez passos e o horizonte corre dez passos. Por mais que eu caminhe, jamais alcançarei. Para que serve a utopia? Serve para isso: para que eu não deixe de caminhar.”
