# Método das Diferenças Finitas aplicado às Equações do Calor e Advecção 
Repositório para o trabalho final de Análise Numérica 


<p align="justify"> Os estudos de ciências naturais são, quase exclusivamente, voltados para a descrição de fenômenos, dos mais raros e ocasionais ao mais cotidianos. O crescimento de um fungo, o movimento de um objeto em queda livre, a colisão de dois corpos, a mudança de fase de uma sustância, são todos episódios descritos por campos específicos, como microbiologia, física clássica, termodinâmica (respectivamente). Contudo, atrelado a cada um destes fenômenos, existe um campo essencial para a análise dos sistemas; a matemática.  Desta forma, através de funções, expressões e conceitos, em conjunto com as leis de cada relativas a cada área, a matemática é capaz de descrever o comportamento de sistemas simples e complexos e sua evolução em relação ao espaço e tempo. </p>

<p align="justify"> Uma forma comum a essas aplicações matemáticas são expressões chamadas equações diferenciais. O princípio básico dessas equações está em relacionar uma função à sua derivada. Um caso particular as equações diferenciais ocorrem quando a expressão apresenta uma derivada parcial de uma função com duas ou mais variáveis independentes. Observa-se que, no exemplo acima, é apresentado uma equação que evolui apenas no tempo, por isso, é chama de Equação Diferencial Ordinária (EDO), no caso da presença de mais variáveis, classificamos como Equação Diferencial Parcial (EDP). A diferença essencial entre os dois casos é que, em EDP’s, além da evolução temporal, pode haver evoluções em uma ou mais dimensões de espaço. </p>

<h3> A equação do calor</h3>

<p align="justify"> A equação do calor, também conhecida como a equação de difusão de calor, é uma equação diferencial parcial que descreve a propagação do calor em um meio. Ela é amplamente utilizada na modelagem de fenômenos de transferência de calor em diversas áreas, como física, engenharia e ciências aplicadas. </p>

$$\frac{\partial u}{\partial t}=k\frac{\partial^2u}{\partial x^2}$$

<h3> A equação de advecção</h3>

<p align="justify" >Por outro lado, a equação de advecção, também conhecida como equação de transporte, é uma equação diferencial parcial que descreve o transporte de uma grandeza ao longo de uma direção específica, geralmente representada pelo eixo x.  </p>

$$ \frac{\partial u}{\partial t}+\mu\frac{\partial u}{\partial x}=0$$

<p align="justify"> Uma forma convencional para aproximar soluções de equações diferenciais parciais, utilizando condições de contorno, dá-se pelo método das Diferenças Finitas, que consiste em discretizar a equação, obtendo assim uma solução numérica, dentro do intervalo pré-posto. Portanto, a aplicação do método consiste na divisão do domínio da função em uma malha, onde a cada ponto será atribuído um valor relacionado a aproximação da derivada naquele ponto. 
A aproximação pode ocorrer no sentido positivo (adiantada) ou negativo (atrasada), visto que se considera para a aproximação dois pontos. Assim, a diferença finita adiantada, toma como base os pontos $x_1$ e $x_2$, sendo ${x_2-x}_1=\ h$, enquanto a diferença finita atrasada toma os pontos $x_0$ e $x_1$, sendo a diferença entre esses dois pontos também igual a $h$. Existe ainda a diferença finita centrada, neste caso, a aproximação considera três pontos. Desta forma, o erro cometido pelo método possui ordem $h$, correspondente ao tamanho do passo dado a cada aproximação. </p>

<p align="justify">  Na equação do Calor, utiliza-se do método FTCS (Forward in Time and Centered in Space). Nesse método, a diferença finita avançada é usada para o tempo e a diferença finita centrada é usada para o espaço. Aplicado o Método das Diferenças Finitas, a equação é discretizada no tempo e no espaço. 
O domínio espacial é dividido em uma malha de pontos, e o tempo é dividido em intervalos regulares. A aproximação da derivada temporal é feita usando a diferença finita avançada, enquanto a aproximação da derivada espacial é feita usando a diferença finita centrada de segunda ordem. Essas aproximações são então substituídas na Equação do Calor, resultando em um sistema de equações discretas. Esse sistema pode ser resolvido numericamente para obter a distribuição de temperatura ao longo do tempo e do espaço.</p>


<p align="justify"> Para aplicar o Método das Diferenças Finitas na Equação de Advecção, a equação é discretizada no tempo e no espaço. O domínio espacial é dividido em uma malha de pontos, e o tempo é dividido em intervalos regulares. A aproximação da derivada temporal é feita usando a diferença finita adiantada, enquanto a aproximação da derivada espacial pode ser feita usando a diferença finita adiantada ou a diferença finita centrada. Essas aproximações são então substituídas na equação, resultando em um sistema de equações discretas. Esse sistema também pode ser resolvido numericamente para obter a evolução da quantidade conservada ao longo do tempo e do espaço. </p>

<h3> Referências </h3>

[1] WASQUES, Vinícius Francisco. Notas Matemáticas: Equações Diferenciais. Ilum Escola de Ciência, 2022. 

[2] MARCELO LOPES VIEIRA. Equações Diferenciais Parciais | Uma Introdução aos Conceitos Básicos (EDPs). Matemática Simplificada. Disponível em: <https://matematicasimplificada.com/equacoes-diferenciais-parciais/>. Acesso em: 24 jun. 2023.

[3] WASQUES, Vinícius Francisco. Notas de Matemática: Análise Numérica. Ilum Escola de Ciência, 2023. 

[4] PEIRCE, A. W. Partial Differential Equations: Lecture 8 - Separation of Variables [PDF]. University of British Columbia, 2012. Disponível em: https://personal.math.ubc.ca/~peirce/M257_316_2012_Lecture_8.pdf. Acesso em: 24 de junho de 2023.

[5] International Centre for Theoretical Physics (ICTP). Aula 10: 2-Numerical Methods for the Advection Equation [PDF]. Disponível em: https://indico.ictp.it/event/a06220/session/18/contribution/10/material/0/2.pdf. Acesso em: 24 de junho de 2023. 


