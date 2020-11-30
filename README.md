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

Devido a simplicidade do problema não é necessário um detalhamento muito elevado. Contudo pelo mesmo motivo relatado acima aumentos na precisão ou detalhamento da simulação não resultaram em tão significativo aumento no tempo de processamento.

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
Quais as condições de contorno a serem utilizadas (Input), o tipo de escoamento (laminar ou turbulento), se será ou não utilizado um modelo de transferência de calor e possíveis alterações na malha ou na geometria.

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


## Descrição do pré-processamento feito no ANSYS:
Para facilitar a organização do processo de “setup” ainda na ferramenta de geração de malha selecionou-se as faces da entrada e saída da geometria e nomeou-as respectivamente “inlet” e “outlet” como a figura seguinte mostra:

![Adição de faces de “inlet” e “outlet”]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Inlet_Outlet.png)

Para facilitar a comparação de resultados com parâmetros diferentes criou-se mais duas “arvores” no workbench utilizando a mesma malha e geometria como a figura seguinte mostra:

![Arvore do workbench]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Arvore_def.png)

Após isso foi definido que o fluido(água), a pressão de referência(atmosférica), o modelo de transferência de calor(nenhum) e o tipo de escoamento(laminar) na etapa de setup de cada uma das arvores. como as figuras seguintes mostram:

![Propriedades do fluido]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Basic%20setting.png)

![Configurações de transferência de calor e turbulência]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/FluidModel.png)

Para finalizar esta etapa em cada uma das arvores foram definidas as condições de contorno na entrada e na saída do cano em cada uma das arvores com os valores discutidos anteriormente (velocidade, pressão e vazão mássica) para assim posteriormente comparar os resultados e ver se convergem ou não.

Definição das condições de entrada com fluxo de massa:

![Seleção da face “inlet”]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Inlet_1.png)

![Entrada por fluxo de massa]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Inlet_2.png)

Definição das condições de saída com fluxo de massa:

![Seleção da face “outlet”]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Outlet_1.png)

![Saída por fluxo de massa]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Outlet_2.png)

# 3- Processamento e Pós-Processamento:

## O histórico de convergência do cálculo está adequado?

Como pode ser observado nas figuras abaixo todas as curvas do gráfico de convergência estão apontadas para baixo, logo o histórico de convergência está adequado.

“Input” e “output” como pressão:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ConvergenciaPressao.png)

“Input” e “output” como vazão mássica: 

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ConvergenciaVelocidade.png)

“Input” como pressão e “output” como vazão mássica:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ConvergenciaVelPressao.png)

## Quanto tempo a simulação está levando para ser processada?
Seguem os tempos de simulação para cada uma das 3 simulações:
“Input” e “output” como pressão: 24,94 segundos.
“Input” e “output” como vazão mássica: 36,588 segundos.
“Input” como pressão e “output” como vazão mássica: 1 minuto 24,677 segundos.
## Os resíduos estão em valores aceitáveis?

Devido a qualidade da malha obtida e a simplicidade da malha os resíduos não apresentaram problemas para esta simulação.

## Resultados obtidos:

Seguem os resultados de cada uma das três simulações realizadas.

### Simulação 1 (“Input” e “output” como vazão mássica):

Vetor velocidade ao longo do escoamento:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/VetorVelocidade1.png)

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ZoomVetorVelocidade1.png)

Distribuição de velocidade:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/DistribVelocidade1.png)

Pressão ao longo do escoamento:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ContornoPressao1.png)

Gráfico da perda de carga:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/PerdaDeCarga1.png)

Gráfico de velocidade: 
![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/PerfilVelocidade1.png)

### Simulação 2 (“Input” e “output” como pressão):

Vetor velocidade ao longo do escoamento:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/VetorVelocidade2.png)

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ZoomVetorVelocidade2.png)

Distribuição de velocidade:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/DistribVelocidade2.png)

Pressão ao longo do escoamento:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ContornoPressao2.png)

Gráfico da perda de carga:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/PerdaDeCarga2.png)

Gráfico de velocidade: 
![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/PerfilVelocidade2.png)

### Simulação 3 (“Input” como pressão e “output” como vazão mássica):

Vetor velocidade ao longo do escoamento:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/VetorVelocidade3.png)

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ZoomVetorVelocidade3.png)

Distribuição de velocidade:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/DistribVelocidade3.png)

Pressão ao longo do escoamento:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/ContornoPressao3.png)

Gráfico da perda de carga:

![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/PerdaDeCarga3.png)

Gráfico de velocidade: 
![]( https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/PerfilVelocidade3.png)

## A simulação fornece resultados qualitativos?

Como as figuras acima mostram há diversos resultados qualitativos obtidos a partir das simulações contudo os mesmos são divergentes.

## É possível calcular resultados quantitativos e qualitativos com o que a simulação calculou?

Sim, a simulação teve como resultado diversos valores como velocidade e pressão a partir dos quais e possível obter valores para propriedades do escoamento como número de Reynolds e número de Mach.

## Os resultados estão de acordo com a realidade física do escoamento?

Houve uma grande discrepância nas simulações quanto a perda de carga, desenvolvimento do escoamento e velocidade, o que indica algum erro na mesma, logo não é possível afirmar que os resultados estão de acordo com a realidade física do escoamento.
