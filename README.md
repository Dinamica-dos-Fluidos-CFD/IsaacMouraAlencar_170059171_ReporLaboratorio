# IsaacMouraAlencar_170059171
Problema 1 -

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também mediu-se a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do do tamanho dos elementos de malha para avaliar se o cenário acima é normal ou não para esta instalação.
# 1- Pre processamento e modelagem:
## Qual é o objetivo do projeto?
O objetivo do projeto é aferir o valor da perda de carga na tubulação apresentada a partir de um estudo paramétrico e comparar este resultado com o apresentado no enunciado do problema e caso haja discrepância dos resultados a partir do estudo paramétrico justificar tal discrepância

## Qual e a finalidade do projeto?
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
Dia 5 de dezembro de 2020

## Há outra metodologia mais adequada do que CFD?
Outra possibilidade para se resolver o problema e a reprodução do mesmo em laboratório, contudo devido a situação da pandemia e a simplicidade CFD e a metodologia mais adequada.

## Requisitos da solução:
O requisito de solução do Projeto de CFD é de confirmar ou não a queda de pressão mencionada no problema a partir de diferentes parâmetros, e caso não seja confirmada mostrar a real queda de pressão assim como justificar a mesma.

## Modelagem:
A primeira etapa do projeto deve ser a modelagem da tubulação que possui 1 metro de comprimento e 40 milímetros de diâmetro, devido a simplicidade da geometria não é necessário nenhuma simplificação ou alteração nesta etapa do projeto, e provavelmente também não será necessário nenhum refino de malha pelo mesmo motivo, contudo não se pode garantir o mesmo das outras etapas.

