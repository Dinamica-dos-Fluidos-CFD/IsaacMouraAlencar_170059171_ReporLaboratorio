# IsaacMouraAlencar_170059171_ReporLaboratorio
Problema 1 - Substituir nota do laboratório.

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também mediu-se a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do do tamanho dos elementos de malha para avaliar se o cenário acima é normal ou não para esta instalação.


# Requisitos:
Aferir a perda de carga na e vazão na instalação descrita, comparar com os valores esperados, justificar qualquer divergência de resultados se existente e com esses resultados realizar um estudo paramétrico da tensão cisalhante na parede do tubo e aferir se tal cenário é normal para esta instalação. Devido a simplicidade do problema não será necessário refinamento de malha ou detalhes da tubulação como material e elementos estruturais visto que tais adições somente aumentariam a demanda de poder computacional sem diferir de maneira significativa o resultado final.

# Simplificações utilizadas na simulação:
Escoamento laminar e isolado(desconsiderando quaisquer trocas de calor com o ambiente)

# Possiveis condições de contorno para serem utilizadas:
Utilizar-se da vazão volumétrica dada pelo problema na entrada e na saída da tubulação, contudo o ansys não aceita vazão volumétrica como condição de contorno, somente vazão mássica, devido a esse problema a vazão volumétrica dada fora multiplicada pela densidade da água(obtida na biblioteca de propriedades materiais do ansys) com valor de 997 kg/m³, obtendo-se o valor de vazão mássica de 0.0997 quilogramas por segundo.
Outra opção e utilizar  a pressão na entrada e saída como condição de contorno, seja utilizando-se de uma pressão manométrica de 2 Pa na entrada do tubo e 0 Pa na saída, ou de 0 Pa na entrada e -2 Pa na saída para comparar os resultados com os obtidos utilizando-se da vazão e aferir se há convergência de resultados ou não.




