# MVP Análise de Dados e Boas Práticas

**Nome:** Paula Alcantara Cardoso

**Matrícula:** 4052025000118

**Dataset:** [Olympic Summer & Winter Games, 1896-2022](https://www.kaggle.com/datasets/piterfm/olympic-games-medals-19862018)

## Descrição do Problema

Os Jogos Olímpicos são o maior evento esportivo mundial, divididos entre as edições de verão e de inverno, que acontecem a cada dois anos. Com o objetivo de promover paz, união e respeito, atletas de todo o mundo competem em mais de 400 eventos.

Originados na Grécia Antiga, os Jogos tinham a finalidade de cultuar os deuses do Olimpo por meio das habilidades dos atletas. Com o crescimento do cristianismo e a ascensão do imperador romano Teodósio, os Jogos foram banidos em 394 d.C., por serem considerados uma festa pagã. Somente em 1896 as competições foram retomadas, dando início aos Jogos Olímpicos da Era Moderna. Os Jogos de Inverno, por sua vez, foram criados em 1924, com foco nos esportes praticados em ambientes frios ou com neve, como o esqui e a patinação no gelo.

Atualmente, além das edições de verão e de inverno, existem também os Jogos Paralímpicos e os Jogos Mundiais da Juventude. No Brasil, há a tradição de acompanhar e torcer pelos atletas nos Jogos de Verão, e nos últimos anos, os Jogos Paralímpicos também têm ganhado maior repercussão.

**REFERÊNCIAS:**

1.  https://www.olympics.com/pt/olympic-games

2.  https://revistagalileu.globo.com/Sociedade/Historia/noticia/2021/07/olimpiadas-conheca-historia-os-simbolos-e-importancia-dos-jogos.html
https://pt.wikipedia.org/wiki/Jogos_Ol%C3%ADmpicos_de_Inverno

## Perguntas do MVP

As perguntas que tracei são as seguintes:
- **Quem são os 5 atletas com mais medalhas nos jogos de verão?**

- **Existe alguma relação entre quantidade de medalhas e participações nos jogos de verão?**

- **Como é a distribuição da quantidade de medalhas por idade dos atletas brasileiros?**

- **Como varia a idade dos atletas medalhistas brasileiros entre as diferentes modalidades esportivas?**

- **Como é a distribuição da idade dos atletas brasileiros medalhistas por edição dos Jogos Olímpicos?**

- **Como a quantidade total de medalhas distribuídas para os atletas brasileiros varia entre as diferentes modalidades esportivas e edições dos Jogos Olímpicos?**

## Desenvolvimento do MVP

Execute o notebook python disponível neste projeto para verificar as etapas de seleção dos dados, a descrição dos atributos do dataset, as importações das bibliotecas e das tabelas do dataset, a análise dos dados e o pré-processamento, as estaísticas descritivas, criação de novos atributos e a visualização dos dados para melhor responder as perguntas aqui propostas.

## Conclusão
Neste trabalho, realizei uma análise exploratória baseada em dados históricos dos Jogos Olímpicos, com o objetivo de investigar o desempenho dos atletas medalhistas e responder a um conjunto de perguntas específicas. A análise partiu de uma base de dados contendo informações sobre atletas, modalidades, tipos de medalha, idade e participações nas edições olímpicas.

As perguntas propostas neste MVP foram:

**Quem são os 5 atletas com mais medalhas nos jogos de verão?**

**Existe alguma relação entre quantidade de medalhas e participações nos jogos de verão?**

**Como é a distribuição da quantidade de medalhas por idade dos atletas brasileiros?**

**Como varia a idade dos atletas medalhistas brasileiros entre as diferentes modalidades esportivas?**

**Como é a distribuição da idade dos atletas brasileiros medalhistas por edição dos Jogos Olímpicos?**

**Como a quantidade total de medalhas distribuídas para os atletas brasileiros varia entre as diferentes modalidades esportivas e edições dos Jogos Olímpicos?**

Antes de processar os dados para buscar a resposta das perguntas, visualizei as primeiras linhas para entender a estrutura geral e os atributos das tabelas do dataset escolhido. Nessa análise, foram identificadas algumas estatísticas como valores mínimo, máximo e médio, instâncias com maior ocorrência nos dados, além de dados inconsistentes e nulos. A partir desse levantamento inicial, pude entender melhor como que os dados estão organizados nas tabelas originais, pude identificar quais atributos seriam essenciais para as minhas análises e comecei a tomar decisões sobre como realizar o pré-processamento dos dados.

Durante o pré-processamento dos dados, selecionei os dados referentes às edições dos jogos de verão, tratei algumas entradas nulas de atletas medalhistas e exclui instâncias que não vinculavam a medalha a um atleta, ou que continha inconsistência, e transformei atributo utilizando one-hot encoding. A minha decisão por não considerar os esportes coletivos (como Futebol, Vôlei, Basquete e muitos outros) foi motivada pela forma como os dados disponíveis trazem apenas as medalhas atribuídas aos países vencedores e não incluem informações detalhadas sobre os atletas de cada equipe — como nome, data de nascimento ou ano da primeira participação olímpica. Como o objetivo do MVP é responder perguntas específicas sobre atletas medalhistas, a ausência dessas informações inviabiliza a inclusão desses casos nas análise. Por consequência, as respostas deste MVP não são verdade absoluta, uma vez que, pela natureza dos dados, diversos atletas e modalidades não tiveram suas medalhas contabilizadas.

Este MVP também abordou as boas práticas de visualização da informação. Ao longo da análise, utilizei diferentes tipos de gráficos para destacar aspectos variados dos dados: gráficos de barras para comparar quantidades de medalhas por atleta e por tipo de medalha; boxplots para comparar distribuições de idade entre modalidades; violinplot para comparar a distribuição da idade dos atletas entre as edições dos jogos; gráficos de dispersão para investigar a relação entre participações e medalhas; e gráficos de heatmap para verificar a quantidade de medalhas entre as modalidades por edições.

Dentre as perguntas propostas, as duas primeiras foram analisadas envolvendo todos os países, com o objetivo de entender o perfil dos atletas mais premiados e a possível correlação entre número de participações e quantidade de medalhas. A partir da terceira pergunta, o foco da análise foi direcionado exclusivamente aos atletas brasileiros, com o intuito de investigar padrões relacionados à idade, modalidade e evolução histórica das conquistas.

As análises revelaram não há uma relação simples e direta entre o número de medalhas ter múltiplas participações olímpicas, e que, entre os brasileiros, há forte concentração de conquistas em modalidades como Judô, Vela e Atletismo. Também foi possível observar diferenças marcantes de idade entre os atletas brasileiros medalhistas de diferentes modalidades — com esportes como Ginástica e Natação premiando atletas mais jovens quando comparado com modalidades como Hipismo e Vela. No mais, a evolução temporal das conquistas mostra que o Brasil tem ampliado seu desempenho nos Jogos Olímpicos, com destaque para as edições mais recentes (Tóquio 2020, Rio 2016 e Londres 2012).

No geral, fiquei bem satisfeita com os resultados que consegui levantar, mesmo com as limitações do dataset. Como é um tema que eu gosto muito, foi divertido pensar nas melhores formas de representar os dados graficamente pra responder às perguntas. Já na fase inicial da exploração, descobri várias curiosidades! Cuidar da parte visual, como escolher cores com significado e entender as escalas e as informações de cada eixo foi uma forma de tentar deixar o MVP mais interessante e com a leitura mais intuitiva. No fim das contas, além de ter sido um exercício técnico, foi um projeto leve e prazeroso de fazer, que explorou o meu lado criativo, que por algum tempo não era tão trabalhado.
