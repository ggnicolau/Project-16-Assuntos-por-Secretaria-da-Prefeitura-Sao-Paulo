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

[[visitors](https://visitor-badge.glitch.me/badge?page_id=ggnicolau.visitor-badge)](https://badges.pufler.dev)
[![Created Badge](https://badges.pufler.dev/created/ggnicolau/Project-7-Hospital-Challenge)](https://badges.pufler.dev)
[![Updated Badge](https://badges.pufler.dev/updated/ggnicolau/Project-7-Hospital-Challenge)](https://badges.pufler.dev)
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

# Assuntos por Secretarias da Prefeitura de São Paulo

## Introdução
Esse projeto é continuação de outros projetos apresentados aqui no GitHub que tratam sobre a Prefeitura de São Paulo.

Temos um projeto que exploramos a API da Secretaria da Fazenda criada pela PRODAM, fazendo análises orçamentárias sobre a terceirização da saúde e da assistência social no Município de São Paulo.

Temos também outros dois projetos que trabalharam em cima da extração de todas as notícias institucionais de todas as secretarias de 2000 a 2019. Um projeto criamos Modelos de Tópicos para cada secretaria, reduzindo a dimensionalidade dos documentos para 30 tópicos; um tópico é um conjunto de palavras hierarquizadas sobre nosso conjunto de documentos e, com isso, conseguimos extrair uma síntese semântica dos assuntos que tratam cada secretaria e sua variação por gestão. Também fizemos um NER, ou seja, extraímos entidades de cada secretaria e gestão para identificar as relações entre agentes públicos, instituições e ações.

## ESSE PROJETO: O que são assuntos?
Já esse projeto utiliza métodos mistos de uma maneira um tanto heterodoxa. Em artigo publicado com Blei para descrever alguns problemas dos modelos de tópicos desenvolvido por ele e sua equipe, nos diz que um dos maiores problemas é definir a melhor quantidade de tópicos para um modelo sobre um Corpus. A tentativa mais assertiva da comunidade para corrigir o problema foi gerar modelos de tópicos aleatoriamente e pedir para especialistas na área do Corpus dizerem qual dos modelos tem melhor representação sobre o assunto, transformando em um modelo supervisionado, algo que chamam de Modelo de Tópicos Interativo (Interactive Topic Model). Há inúmeras propostas interativas, como as de Li & McCallum (2007), Chang & Boyd-Graeber(2009). Hu & Boyd-Graeber (2014), Lund (2017), Dasgupta (2019).

Nosso trabalho foi uma conclusão de Doutorado de 5 anos. Desses cinco anos, três foram dedicados a etnografia política (observação participante). Estivemos ativos diariamente em ocupações urbanas da população de rua, movimentos de moradia em geral, movimentos de direitos humanos, movimentos de favelas e movimentos de trabalhadores no serviço público (muitos terceirizados) de diversos tipos. Ali pudemos entender também, junto com a nossa formação acadêmica em ciência política, quais são os assuntos, termos e significados dados às palavras, seja pelas Secretarias do Município de São Paulo ou seja pelas pessoas e movimentos engajados nos assuntos da Cidade.

Junto com colegas de profissão e também dos movimentos sociais, também adaptamos a proposta do Blei para um modelo supervisionado. Ao invés de gerar o modelo de tópicos não-supervisionado, criamos os nossos próprios tópicos sobre determinados assuntos (a partir de agora denominamos esse tipo definição de 'assunto'). Ou seja, um assunto é um conjunto de palavras definido por especialistas. E projetamos esses assuntos no nosso Corpus de Documentos, ou seja, projetamos nossos assuntos nas notícias institucionais oficiais de todas as Secretarias do Município de São Paulo, assim como faríamos com o modelo de tópicos para retornar sentidos e relações sobre o nosso Corpus, reduzindo sua dimensionalidade.

## Resultados
Criamos os seguintes assuntos:
* Armas de Fogo
* Assistência Social
* D.B.A.
* D.H.
* Drogas
* Habitação
* Pop Rua
* Saúde
* Saúde Mental
* Segurança
* Trabalho

Assim, podemos criar gráficos de análise para verificar a variação no tempo da quantidade de documentos emitidos para cada assunto e também verificar a intersecção entre assuntos variando no tempo. Por intersecção de assuntos entendemos um documento que fala simultaneamente de um assunto e de outro assunto. Gera-se um gráfico como esse:



Como conclusões gerais analisando todos os gráficos temos:
* Quando se fala de ambulantes, sempre o assunto é segurança; quando mais se falou de ambulantes foi em 2013;
* Quando se fala de Armas de Fogo, 60% em média é junto com DH (desarmamento) durante a gestão Haddad e 10% em média nas outras gestões; entre 2014 e 2015 foi o momento que mais se falou de Armas de Fogo (Desarmamento, nesse contexto);
* Quando se fala de DH, 2% é sobre desarmamento;
* Quando se fala de Armas de Fogo, 10% em média (por trimestre) é com segurança durante todas as gestões, mas com um pico de 15% no último trimestre de 2015;
* Quando se fala de Assistência Social, 25% em média se falava sobre Pop Rua na gestão Kassab, caindo para 10% na gestão Haddad e chegando a quase 35% na gestão Dória/Covas; se falou mais de Assistência Social entre 2014 e 2017;
* Quando se fala de Assistência Social, 15% em média se falou de Segurança entre 2012 e 2014 (pauta Cracolândia esteve na Mídia e programas foram substituídos e tendados), mas depois voltou à média de 8%;
* Quando se fala de D.B.A, mais de 55% se fala de Direitos Humanos, depois foi abandonado o programa na gestão Dória/Covas e quando se falava 30% era sobre DH; se falou mais de DBA no segundo trimestre de 2016;
* Quando se fala de DBA por volta de 60% é diretamente sobre população de rua; quando se fala de DBA, por volta de 7% é sobre segurança;
* Quando se fala de DH, por volta de 5% é sobre DBA durante a gestão Haddad;
* Se falava o dobro sobre DH na Gestão Haddad do que na Gestão Dória/Covas, mas enquanto 8% era sobre Pop Rua na Gestão Haddad, era 16% na Gestão Dória/Covas;
* Quando se fala de DH, por volta de 15% é na gestão Haddad e cai durante a gestão Dória/Covas;
* Quando se fala de Drogas, por volta de 20% se fala sobre Pop Rua, com um pico de 30% no segundo trimestre de 2016;
* Sempre que se fala sobre Drogas, se fala sobre Saúde;
* Por volta de 40% do que se falou sobre Drogas se falou também sobre Saúde Mental em 2014, caindo progressivamente para 20% em 2018;
* Quando se falou de Habitação 14% era sobre Mananciais em 2010, voltando o assunto somente entre meados de 2015 a 2017 com 6%; quando se fala sobre Mananciais sempre se fala sobre Habitação e nunca se fala sobre Segurança;
* Quando se fala de Habitação em média 5% se fala sobre Pop Rua, com um pico de 13% no terceiro trimestre de 2018 para em seguida voltar ao normal;
*  Quando se fala de Pop Rua por volta de 80% se fala de Assistência Social, sendo entre 2016 e 2018 o momento que mais se falou sobre Pop Rua (mais especificamente meados de 2018);
*  Quando se falou de Pop Rua a Gestão Haddad chegou a falar 60% de Direitos Humanos (criou a Secretaria de DH);
*  Quando se fala de Pop Rua entre 2013 e 2017 chegou a se falar 40% de Drogas (2015), caindo para 10% ou desaparecendo posteriormente;
*  A relação Pop Rua com Drogas e Seguranças simultaneamente teve seu ápice em 2015 com 4% e durou de 2014 a 2017;
*  Quando se falou de Pop Rua no início de 2012, 30% se falava de Habitação, caindo progressivamente nos anos seguintes e acentuadamente em 2016;
* Quando se falou de Pop Rua entre 2013 a 2016, por volta de 50% se falava sobre Saúde Geral, caindo acentuadamente o assunto nos anos seguintes;
*  Começa a se falar de Pop Rua com Segurança em 2010, mas começa a crescer em 2012, chegando a 10% de intersecção no segundo trimestre de 2014, se estabilizando em 6% nos anos seguintes;
* A intersecção de Pop Rua com DBA e Segurança acontece entre 2014 e 2017, com ápice em meados de 2015, chegando a 4%;
* Já a intersecção de Pop Rua com Trabalho é praticamente constante de 2014 a 2017 em 80%, caindo para ainda relevantes 70% nos anos seguintes;
* Quando se falou de Segurança se falou 20% de ambulantes no final de 2009 e só voltou a se falar em 2013 com uma taxa média variável de 10%;
* Quando se falou de Segurança se falou de Assistência Social numa taxa constante de 10% de 2013 em diante;
* Em 2013, quando se falou de Segurança, se falou também de DH em 30% das vezes, caindo constantemente até 10% em 2018;
* Quando se falou de Segurança, se falou 1% de Pop Rua, tendo um salto abrupto para 4% no final de 2017 e subindo nos anos seguintes para quase 20% (!?);
* Os Viadutos passam a ser um assunto central da Segurança a partir de 2013, tendo seu ápice entre 2015 e 2016 correspndendo a mais de 60% e caindo para 40% no final de 2017;
* Segurança nunca fala de Mananciais;
* De 2013 ao final de 2018 se falou progressivamente de Trabalho para Pop Rua, chegando a corresponder 20% das vezes que se falou de Trabalho;
* Enquanto quando que se falou de Viaduto apenas 1% era sobre Pop Rua, entre 90% e 100% das vezes que se falou de Viadutos foi para falar de Segurança;

[<span style="font-size:1.5em;"Clique aqui se quiser ver todos os gráficos gerados. </span>](https://github.com/ggnicolau/Project-7-Hospital-Challenge/blob/main/presentation.md)

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



## Arquivos
* Conclusion Report: https://github.com/ggnicolau/Project-7-Hospital-Challenge/tree/main/conclusion_report
* Repository: https://github.com/ggnicolau/Albert_Einstein
* Python Files: https://github.com/ggnicolau/Albert_Einstein/tree/main/py_files
* Profiling Report:  https://github.com/ggnicolau/Albert_Einstein/tree/main/Profiling_report
* Pictures: https://github.com/ggnicolau/Albert_Einstein/tree/main/Pictures
* Pickle Files: https://github.com/ggnicolau/Albert_Einstein/tree/main/Models_backup


## Technical articles
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

## Versioning

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
