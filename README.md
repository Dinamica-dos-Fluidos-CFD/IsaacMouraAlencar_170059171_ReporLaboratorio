# IsaacMouraAlencar_170059171_ReporLaboratorio
Problema 1 - Substituir nota do laboratório.

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também mediu-se a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do do tamanho dos elementos de malha para avaliar se o cenário acima é normal ou não para esta instalação.


# Objetivo:
Aferir a perda de carga na tubulação descrita acima, comparar com o valor esperado, e justificar qualquer divergência de resultados se existente.

# Simplificações utilizadas na simulação:
Escoamento laminar e isolado(desconsiderando quaisquer trocas de calor com o ambiente)

# Geometria utilizada:
![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/geometria.png)

# Detalhes da malha utilizada:
Devido a simplicidade do problema apresentado não foram feitas modificações a malha padrão do ansys.
![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Malha1.png)
![](https://github.com/Dinamica-dos-Fluidos-CFD/IsaacMouraAlencar_170059171_ReporLaboratorio/blob/master/Malha2.png)

# Condições de contorno utilizadas e como foram obtidas:
De início planejava-se utilizar-se da vazão volumétrica dada pelo problema na entrada e na saída da tubulação, contudo o ansys não aceita vazão volumétrica como condição de contorno, somente vazão mássica, devido a esse problema a vazão volumétrica dada fora multiplicada pela densidade da água(obtida na biblioteca de propriedades materiais do ansys) com valor de 997 kg/m³, obtendo-se o valor de vazão mássica de 0.0997 kilogramas por segundo.
