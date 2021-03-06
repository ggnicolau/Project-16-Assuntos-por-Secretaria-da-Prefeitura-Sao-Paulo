<div align="center">
<img src="https://coursereport-production.imgix.net/uploads/school/logo/84/original/logo-ironhack-blue.png?w=200&h=200&dpr=1&q=75">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTx0OPgRAs3027QxPjMtXI-1UtLxObz5x6rpvb5bVfEASQJ19fs9Bi14CLOOwwhtJoYXw&usqp=CAU">
</div>


<div align="left">

[![](https://readme-typing-svg.herokuapp.com/)](https://git.io/typing-svg)
</div>
<!--GITHUB_ACTIVITY:{"rows": 5}-->

---

<div align="center">

[![visitors](https://visitor-badge.glitch.me/badge?page_id=ggnicolau.visitor-badge)](https://badges.pufler.dev)
[![Created Badge](https://badges.pufler.dev/created/ggnicolau/Project-16-Assuntos-por-Secretaria-da-Prefeitura-Sao-Paulo)](https://badges.pufler.dev)
[![Updated Badge](https://badges.pufler.dev/updated/ggnicolau/Project-16-Assuntos-por-Secretaria-da-Prefeitura-Sao-Paulo)](https://badges.pufler.dev)
[![Commits Badge](https://badges.pufler.dev/commits/monthly/ggnicolau)](https://badges.pufler.dev)
[![Repos Badge](https://badges.pufler.dev/repos/ggnicolau)](https://badges.pufler.dev)
[![Years Badge](https://badges.pufler.dev/years/ggnicolau)](https://badges.pufler.dev)
[![ggnicolau StackOverflow](https://stackoverflow-badge.vercel.app/?userID=15673147)](https://stackoverflow.com/users/15673147/ggnicolau)

![+5511976431347](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)
![ggnicolau](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)
![ggnicolau@usp.br](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![https://www.linkedin.com/in/ggnicolau/](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)
![Python 3.9](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![pgAdmin](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Atom](https://img.shields.io/badge/Atom-66595C?style=for-the-badge&logo=Atom&logoColor=white)
![Windows 10 Pro](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=ggnicolau&show_icons=true&theme=darcula)
</div>
<!--GITHUB_ACTIVITY:{"rows": 5}-->

---

<div align="left">
<div class=''text-justify''>

# Assuntos por Secretarias da Prefeitura de S??o Paulo

#### Technologies
* Python version  3.9
* R
* Excel
* MongoDB
* Git

#### Tools
* Atom
* VS Studio
* Jupyter IPython

#### Services
* Github

## Introdu????o
Esse projeto ?? continua????o de outros projetos apresentados aqui no GitHub que tratam sobre a Prefeitura de S??o Paulo.

Temos um projeto que exploramos a API da Secretaria da Fazenda criada pela PRODAM, fazendo an??lises or??ament??rias sobre a terceiriza????o da sa??de e da assist??ncia social no Munic??pio de S??o Paulo.

Temos tamb??m outros dois projetos que trabalharam em cima da extra????o de todas as not??cias institucionais de todas as secretarias de 2000 a 2019. Um projeto criamos Modelos de T??picos para cada secretaria, reduzindo a dimensionalidade dos documentos para 30 t??picos; um t??pico ?? um conjunto de palavras hierarquizadas sobre nosso conjunto de documentos e, com isso, conseguimos extrair uma s??ntese sem??ntica dos assuntos que tratam cada secretaria e sua varia????o por gest??o. Tamb??m fizemos um NER, ou seja, extra??mos entidades de cada secretaria e gest??o para identificar as rela????es entre agentes p??blicos, institui????es e a????es.

## O que s??o assuntos?
J?? esse projeto utiliza m??todos mistos de uma maneira um tanto heterodoxa. Em artigo publicado por David Blei (2010) para descrever alguns problemas dos modelos de t??picos desenvolvido por ele e sua equipe, nos diz que um dos maiores problemas ?? definir a melhor quantidade de t??picos para um modelo sobre um Corpus. A tentativa mais assertiva da comunidade para corrigir o problema foi gerar modelos de t??picos aleatoriamente e pedir para especialistas na ??rea do Corpus dizerem qual dos modelos tem melhor representa????o sobre o assunto, transformando em um modelo supervisionado (BLEI, 2010), algo que chamam de Modelo de T??picos Interativo (Interactive Topic Model). H?? in??meras propostas interativas, como as de Li & McCallum (2007), Chang & Boyd-Graeber(2009). Hu & Boyd-Graeber (2014), Lund (2017), Dasgupta (2019).

Nosso trabalho foi uma conclus??o de Doutorado de 5 anos. Desses cinco anos, tr??s foram dedicados a etnografia pol??tica (observa????o participante). Estivemos ativos diariamente em ocupa????es urbanas da popula????o de rua, movimentos de moradia em geral, movimentos de direitos humanos, movimentos de favelas e movimentos de trabalhadores no servi??o p??blico (muitos terceirizados) de diversos tipos. Ali pudemos entender tamb??m, junto com a nossa forma????o acad??mica em ci??ncia pol??tica, quais s??o os assuntos, termos e significados dados ??s palavras, seja pelas Secretarias do Munic??pio de S??o Paulo ou seja pelas pessoas e movimentos engajados nos assuntos da Cidade.

Junto com colegas de profiss??o e tamb??m dos movimentos sociais, tamb??m adaptamos a proposta do Blei para um modelo supervisionado. Ao inv??s de gerar o modelo de t??picos n??o-supervisionado, criamos os nossos pr??prios t??picos sobre determinados assuntos (a partir de agora denominamos esse tipo defini????o de 'assunto'). Ou seja, um assunto ?? um conjunto de palavras definido por especialistas. E projetamos esses assuntos no nosso Corpus de Documentos, ou seja, projetamos nossos assuntos nas not??cias institucionais oficiais de todas as Secretarias do Munic??pio de S??o Paulo, assim como far??amos com o modelo de t??picos para retornar sentidos e rela????es sobre o nosso Corpus, reduzindo sua dimensionalidade.

Em etapas anteriores trabalhamos m??todos qualitativos (etnografia pol??tica e observa????o participante), m??todos quantitativos (estat??stica explorat??ria or??ament??ria e modelos lingu??sticos n??o-supervisionados). Nossa inten????o era somar os m??todos e saltar do indutivo ao dedutivo ('Problema de Plat??o'), integrando a uma teoria (isso est?? posto em nossa Tese de Doutorado). Entendemos esse ??ltimo modelo apresentado aqui, supervisionado por especialistas e com aux??lio da m??quina, uma an??lise intersubjetiva feita com olhar especializado, que acrescenta um elemento Reflexivista ?? nossa an??lise.

## Resultados
Criamos os seguintes assuntos:
* Armas de Fogo
* Assist??ncia Social
* D.B.A.
* D.H.
* Drogas
* Habita????o
* Pop Rua
* Sa??de
* Sa??de Mental
* Seguran??a
* Trabalho

Assim, podemos criar gr??ficos de an??lise para verificar a varia????o no tempo da quantidade de documentos emitidos para cada assunto e tamb??m verificar a intersec????o entre assuntos variando no tempo. Por intersec????o de assuntos entendemos um documento que fala simultaneamente de um assunto e de outro assunto. Gera-se um gr??fico como esse:

<div align="center">
<img src="https://github.com/ggnicolau/Project-16-Assuntos-por-Secretaria-da-Prefeitura-Sao-Paulo/blob/main/Graphs/armas_DH.png">
</div>

Como conclus??es gerais analisando todos os gr??ficos temos:
* Quando se fala de ambulantes, sempre o assunto ?? seguran??a; quando mais se falou de ambulantes foi em 2013;
* Quando se fala de Armas de Fogo, 60% em m??dia ?? junto com DH (desarmamento) durante a gest??o Haddad e 10% em m??dia nas outras gest??es; entre 2014 e 2015 foi o momento que mais se falou de Armas de Fogo (Desarmamento, nesse contexto);
* Quando se fala de DH, 2% ?? sobre desarmamento;
* Quando se fala de Armas de Fogo, 10% em m??dia (por trimestre) ?? com seguran??a durante todas as gest??es, mas com um pico de 15% no ??ltimo trimestre de 2015;
* Quando se fala de Assist??ncia Social, 25% em m??dia se falava sobre Pop Rua na gest??o Kassab, caindo para 10% na gest??o Haddad e chegando a quase 35% na gest??o D??ria/Covas; se falou mais de Assist??ncia Social entre 2014 e 2017;
* Quando se fala de Assist??ncia Social, 15% em m??dia se falou de Seguran??a entre 2012 e 2014 (pauta Cracol??ndia esteve na M??dia e programas foram substitu??dos e tendados), mas depois voltou ?? m??dia de 8%;
* Quando se fala de D.B.A, mais de 55% se fala de Direitos Humanos, depois foi abandonado o programa na gest??o D??ria/Covas e quando se falava 30% era sobre DH; se falou mais de DBA no segundo trimestre de 2016;
* Quando se fala de DBA por volta de 60% ?? diretamente sobre popula????o de rua; quando se fala de DBA, por volta de 7% ?? sobre seguran??a;
* Quando se fala de DH, por volta de 5% ?? sobre DBA durante a gest??o Haddad;
* Se falava o dobro sobre DH na Gest??o Haddad do que na Gest??o D??ria/Covas, mas enquanto 8% era sobre Pop Rua na Gest??o Haddad, era 16% na Gest??o D??ria/Covas;
* Quando se fala de DH, por volta de 15% ?? na gest??o Haddad e cai durante a gest??o D??ria/Covas;
* Quando se fala de Drogas, por volta de 20% se fala sobre Pop Rua, com um pico de 30% no segundo trimestre de 2016;
* Sempre que se fala sobre Drogas, se fala sobre Sa??de;
* Por volta de 40% do que se falou sobre Drogas se falou tamb??m sobre Sa??de Mental em 2014, caindo progressivamente para 20% em 2018;
* Quando se falou de Habita????o 14% era sobre Mananciais em 2010, voltando o assunto somente entre meados de 2015 a 2017 com 6%; quando se fala sobre Mananciais sempre se fala sobre Habita????o e nunca se fala sobre Seguran??a;
* Quando se fala de Habita????o em m??dia 5% se fala sobre Pop Rua, com um pico de 13% no terceiro trimestre de 2018 para em seguida voltar ao normal;
*  Quando se fala de Pop Rua por volta de 80% se fala de Assist??ncia Social, sendo entre 2016 e 2018 o momento que mais se falou sobre Pop Rua (mais especificamente meados de 2018);
*  Quando se falou de Pop Rua a Gest??o Haddad chegou a falar 60% de Direitos Humanos (criou a Secretaria de DH);
*  Quando se fala de Pop Rua entre 2013 e 2017 chegou a se falar 40% de Drogas (2015), caindo para 10% ou desaparecendo posteriormente;
*  A rela????o Pop Rua com Drogas e Seguran??as simultaneamente teve seu ??pice em 2015 com 4% e durou de 2014 a 2017;
*  Quando se falou de Pop Rua no in??cio de 2012, 30% se falava de Habita????o, caindo progressivamente nos anos seguintes e acentuadamente em 2016;
* Quando se falou de Pop Rua entre 2013 a 2016, por volta de 50% se falava sobre Sa??de Geral, caindo acentuadamente o assunto nos anos seguintes;
*  Come??a a se falar de Pop Rua com Seguran??a em 2010, mas come??a a crescer em 2012, chegando a 10% de intersec????o no segundo trimestre de 2014, se estabilizando em 6% nos anos seguintes;
* A intersec????o de Pop Rua com DBA e Seguran??a acontece entre 2014 e 2017, com ??pice em meados de 2015, chegando a 4%;
* J?? a intersec????o de Pop Rua com Trabalho ?? praticamente constante de 2014 a 2017 em 80%, caindo para ainda relevantes 70% nos anos seguintes;
* Quando se falou de Seguran??a se falou 20% de ambulantes no final de 2009 e s?? voltou a se falar em 2013 com uma taxa m??dia vari??vel de 10%;
* Quando se falou de Seguran??a se falou de Assist??ncia Social numa taxa constante de 10% de 2013 em diante;
* Em 2013, quando se falou de Seguran??a, se falou tamb??m de DH em 30% das vezes, caindo constantemente at?? 10% em 2018;
* Quando se falou de Seguran??a, se falou 1% de Pop Rua, tendo um salto abrupto para 4% no final de 2017 e subindo nos anos seguintes para quase 20% (!?);
* Os Viadutos passam a ser um assunto central da Seguran??a a partir de 2013, tendo seu ??pice entre 2015 e 2016 correspndendo a mais de 60% e caindo para 40% no final de 2017;
* Seguran??a nunca fala de Mananciais;
* De 2013 ao final de 2018 se falou progressivamente de Trabalho para Pop Rua, chegando a corresponder 20% das vezes que se falou de Trabalho;
* Enquanto quando que se falou de Viaduto apenas 1% era sobre Pop Rua, entre 90% e 100% das vezes que se falou de Viadutos foi para falar de Seguran??a;

[<span style="font-size:1.5em;">Clique aqui se quiser ver todos os gr??ficos gerados. </span>](https://github.com/ggnicolau/Project-16---Assuntos-por-Secretaria-da-Prefeitura-S-o-Paulo/tree/main/Graphs)


## Arquivos

* Gr??ficos Selecionados: https://github.com/ggnicolau/Project-16-Assuntos-por-Secretaria-da-Prefeitura-Sao-Paulo/tree/main/Graphs
* Tabela em Excel com todas as informa????es (voc?? mesmo pode fazer suas an??lises comparativas): https://github.com/ggnicolau/Project-16-Assuntos-por-Secretaria-da-Prefeitura-Sao-Paulo/tree/main/Excel_file

## Artigos T??cnicos
* https://arxiv.org/pdf/1907.05545.pdf
* http://www.cs.columbia.edu/~blei/papers/Blei2012.pdf
* https://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf
* http://journalofdigitalhumanities.org/2-1/topic-modeling-and-digital-humanities-by-david-m-blei/
* https://papers.nips.cc/paper/2007/file/d56b9fc4b0f1be8871f5e1c40c0067e7-Paper.pdf
* https://www.cs.umd.edu/sites/default/files/scholarly_papers/YueningHu_1.pdf
* https://aclanthology.org/W15-1212.pdf
* https://arxiv.org/pdf/1907.04919.pdf
* https://aclanthology.org/P11-1026.pdf
* http://ciir.cs.umass.edu/pubfiles/ir-512.pdf
* https://papers.nips.cc/paper/2009/file/f92586a25bb3145facd64ab20fd554ff-Paper.pdf

## Outros Reposit??rios da minha Tese de Doutorado:
* https://github.com/ggnicolau/Project-5-NLP-SP-City-Hall
* https://github.com/ggnicolau/Project-9-NER-SP-City-Hall
* https://github.com/ggnicolau/Project-2-API_Secretaria-da-Fazenda
* https://github.com/ggnicolau/Project-10-TuneLDA-SP-City-Hall

## Versionamento

1.0.0.0

## Autor

* **Guilherme Giuliano Nicolau**: @ggnicolau (https://github.com/ggnicolau)

</div>

<!--GITHUB_ACTIVITY:{"rows": 5}-->

---

<div align="center">

<br/><br/>
![Quote](https://github-readme-quotes.herokuapp.com/quote?theme=dark&animation=grow_out_in)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ggnicolau&layout=compact)](https://github.com/anuraghazra/github-readme-stats)

![https://medium.com/@ggnicolau](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)


</div>
