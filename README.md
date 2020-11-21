# IsaacMouraAlencar_170059171
Problema 1 -

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também se mediu a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do tamanho dos elementos de malha para avaliar se o cenário acima é normal ou não para esta instalação.
# 1- Modelagem:
## Qual é o objetivo do projeto?
O objetivo do projeto é aferir o valor da perda de carga na tubulação apresentada a partir de um estudo paramétrico e comparar este resultado com o apresentado no enunciado do problema. Em caso de discrepância dos resultados justificar tal discrepância a partir do estudo paramétrico e da literatura disponível.

## Qual é a finalidade do projeto?
O projeto tem fim acadêmico de modo que demonstre a visualização do escoamento citado e dos parâmetros através da simulação computacional e de cálculos feitos utilizando a teoria de Dinâmica dos Fluidos para se caracterizar o escoamento e confirmar os resultados obtidos de cada forma.

## Que hipóteses de simplificação podem ser adotadas?
O escoamento será considerado laminar devido às características do fluido e do tubo e para a facilitação dos cálculos do problema.
A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação, porém, não complexa demais para a demanda do problema.
O problema considera regime permanente.
Trocas de calor não serão consideradas.
Filtrar os parâmetros que necessitam de simulação para averiguar o problema e efetuar os cálculos, para assim não haver simulações desnecessárias.

## Que hipóteses de simplificação devem ser adotadas?
O escoamento será considerado laminar devido às características do fluido e do tubo.
A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação, porém, não complexa demais para a demanda do problema.
O problema considera regime permanente.
Trocas de calor não serão consideradas

## Qual é a precisão requerida nos resultados do projeto?
Devido a simplicidade do problema onde há uma suposta perda de carga de 2 Pa, a precisão requerida deve ser de duas a três casas decimais, já que desse modo não será necessário muito poder computacional assim como caso a perda de carga seja próxima da relatada no problema variações menores que isso seriam de impacto pequeno.

## Qual é o prazo de entrega do projeto?
Dia 4 de dezembro de 2020

## Há outra metodologia mais adequada do que CFD?
Outra possibilidade para se resolver o problema e a reprodução do mesmo em laboratório reproduzindo o modelo descrito no problema. Contudo devido a situação da pandemia e a simplicidade do problema, o CFD se torna uma opção mais atraente, mas não necessariamente a mais adequada.

## Requisitos da solução:
O requisito de solução do Projeto de CFD é a vazão e pressão no interior da instalação mencionada. Com estes valores, será executado um estudo paramétrico de modo a avaliar se estes resultados são suficientes para atender os objetivos.
## Geometria:

![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/geometria.png)


## Desenho esquemático da modelagem do problema:

![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Esquema.png)

# 2- Pré-processamento:

## 	Quanto detalhado o domínio de cálculo precisa ser?

Devido a simplicidade do problema não é necessário um detalhamento muito elevado. Contudo pelo mesmo motivo relatado acima, será possível um detalhamento maior caso o mesmo seja necessário em virtude de algum problema com os resultados ou com o estudo paramétrico.

## 	A geometria está adequada?

A geometria foi feita com as dimensões exatas relatadas no problema sem necessidade de qualquer simplificação ou alteração, logo a mesma está adequada.

## 	Que tipo de malha e método usar? Estruturada ou não-estruturada? Volumes Finitos ou Elementos Finitos?

Devido a simplicidade da geometria e a simplicidade do problema a malha a ser utilizada será a gerada automaticamente pelo programa (hexaédrica simples e estruturada), visto que ela possui bons valores de “Skewness” e de qualidade ortogonal. O método dos volumes finitos será utilizado pois o mesmo faz cálculos baseados na energia, massa e quantidade de movimento em cada volume determinado.

## 	Quais são as informações de entrada (Input) do problema?
Para esta etapa existem diversos possíveis “inputs” que podem ser utilizados como:
Pressões na entrada e saída da tubulação (com queda de 2 pa).
Vazão mássica (calculada a partir da vazão volumétrica).
Velocidade média do escoamento (calculada a partir da área e da vazão volumétrica).

## 	Que escolhas devem ser feitas em relação ao processamento da solução?
Quais as condições de contorno a serem utilizadas.

## 	Quais são os prazos e disponibilidade de capacidade computacional para a análise em questão?

Como o prazo final deste relatório é no dia 4 de dezembro o ideal e que a simulação esteja pronta para o pós processamento uma semana antes.
As especificações do computador a ser utilizado para a simulação são as seguintes:
Processador Intel® Core™ i5-4440 CPU @ 3.10 GHz 3.10 GHz.
Memória instalada 8,0 GB.
Placa de vídeo Nvidia GTX 1050 TI.
Sistema operacional: Windows 10 home.

## Malha e qualidade obtidos:

![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Malha2.png)

![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Malha1.png)

![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Skewness.png)

![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Orthogonal_quality.png)

