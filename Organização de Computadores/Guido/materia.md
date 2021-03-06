#ORGANIZAÇÃO DE COMPUTADORES
_____________________________


## 1. Caracterização do Hardware Computacional: Componentes e Circuitos.

A caracterização dos diversos componentes que são utilizados em um sistema de computadores deve ser feita, antes de mais nada, com base nos grupos elétrico existentes: **condutores de eletricidade**, **isolantes de eletricidade** e **semi-condutores de eletricidade**. Destacamos ainda que todo condutor de eletricidade, isto é, todo material que possui muitos elétrons livres, tal como o cobre, é também um bom condutor térmico. Por outro lado, bons condutores térmicos não são necessariamente bons condutores elétricos, tal como ocorre com um plástico especial chamado de mica que por essa característica é amplamente empregado em computadores e outros aparelhos eletro eletrônicos, visando conectar mecanicamente um componente eletrônico com a sua chapa metálica dissipadora de calor, isolando-os eletricamente.
Além da caracterização elétrica básica mencionamos nesse curso questões físicas um pouco mais atuais que podem ajudar a explicar o funcionamento de determinados componentes e fenomenos, que ao longo das próximas décadas, devem começar a viabilizar na prática o que se conhece por **computação quântica**, que deve ser tratado com um paradigma distinto do atual. Neste aspecto, a anti-matéria ja possui papel importante, a exemplo, do que utilizamos na medicina avançada, exemplificado por um exame para diagnóstico preciso de tumores chamado de **PET-SCAN**(tecnoglogia de emissão de pósitrons). Neste exame a anti-matéria do elétron(pósitron), isto é, elétron com carga positiva, é a base do funcionamento.
Além dos conceitos mencionados devemos também dar particular atenção aos processos que envolvem a matéria física e seu quarto estado que é plasmático. Quando temos um sólido perfeitamente caracterizado, tal como um bloco de gelo, podemos aquece-lo de forma que as moléculas de água que estavam mais fortemente conectadas ficam um pouco mais soltas conduzindo ao estado líquido. Prosseguindo no aquecimento, as moléculas de água ficam ainda mais desunidas, obtendo-se então o estado gasoso. Se prosseguirmos aquecendo o material, até atingir temperaturas extremamente altas, chegamos a um estado, chamado **plasmático**, em que não somente as moléculas estão muito dissosiadas, mas os próprios átomos se descaracterizam. Esse conjunto de partículas dissosiadas, que formam o plasma, é consideravelmente instável e normalmente **condutor de eletricidade**, ja que existe consideravel quantidade de elétrons livres. Importante ainda é resaltar que não somente o aquecimento extremo conduz ao plasma pois um campo elétrico também pode ter potencial para dissosiar partículas de um gás fazendo com que ele atinga o quarto estado da matéria(plasmático), tal como ocorre em alguns tipos de lâmpadas por exemplo. Neste curso, consideramos o estado plasmático para fins de projeto e frabricação de componentes eletrônicos tais como os circuitos integrados, conforme veremos adiante.
Destacamos ainda o conceito de **litografia**, que constitui um tipo de arte, isto é desenho, em uma superfície sólida, de modo a depositar partículas em um determinado material para que ele passe a possuir as características elétricas desejadas. Normalmente a litografia é utilizada na construção de componentes e circuitos integrados em escala micro ou nanoscópica, utilizando-se um feixe de elétrons para realizar a deposição de materiais químicos. Sendo assim, é comum utilizarmos o termo litografia por feixe de elétrons. 

Passamos agora a recordar e caracterizar eletricamente os principais componentes que constituem os circuitos eletronicos digitais e em seguida reuniremos os conceitos para compreender processos de fabricação.

 - **Resistência ohmica**: caracterizada nos resistores eletrônicos, constitue um comportamento não reativo, isto é independente da duração ou da frequência do sinal elétrico que atravessa o componente. Utilizaremos, seguindo o padrão a letra `R` para menciona-la.

 - **Indutância elétrica**: caracterizada por meio dos indutores, popularmente conhecidos como bubinas, caracteriza-se por um elemento reativo, isto é um elemento que oferece oposição a passagem da corrente elétrica, sendo que esta oposição muda de acordo com a duração ou a frequência do sinal elétrico que o atravessa. Simbolizando por `L` o valor de uma indutância, que é medida em Henry, quantificamos a oposição que um indutor oferece a passagem da corrente elétrica por `ω.L` sendo omega `ω` a frequência do sinal elétrico que atravessa a indutância.

 - **Capacitância**: caracterizada nos componentes conhecidos como capacitores, oferece resistência, ou seja, oposição a passagem da corrente elétrica também de modo reativo, sendo essa oposição quantificada por `1/ ω.C` em que `C` é o valor do capacitor em Farads.

De acordo com os três elementos definidos acima, caracterizamos o termo conhecido como **impedância**, medida em ohms, como a soma de três forças contrárias à passagem da corrente elétrica: **resistência**, **indutância** e **capacitância**. A primeira, normalmente obtida utilizando-se pistas de carvão litografadas em um sólido, a segunda espiras de fio condutor em torno de um núcleo em que gera um campo magnético na tentativa de impedir variações da corrente elétrica e a terceira operando de modo semelhante por meio de duas placas condutoras separadas por um material isolante que forma um campo elétrico entre suas placas. Concluindo, denotamos por `Z` a impedância total, com suas partes resistiva, indutiva e capacitiva.


**<p align="center"> Z = Zr + Zl + Zc </p>**

-------------------------------------------

# Exemplos:

### 1. Caracterize a impedância resistiva de um resistor de 100ohms quando ele é atravessado por um sinal senoidal de amplitude +-1V com frequência de 10Hz.

### Solução:

>	Z = 100ohms, pois resistencia não é reativa e assim frequencias e amplitudes dos sinais que atravessam em nada alteram a oposição que o componente oferece.

### 2. Caracterize a impedância indutiva de uma bubina de ½ Henry, quando percorrida por um sinal elétrico de 100Hz, senoidal, com amplitudes +-5V.

### Solução:

>		Zl = ω.L
>		Zl = 2.pi.f.L
>		Zl = 2.3,1415.100.0,5 = 314 ohms

>Obs: a amplitude do sinal que atravessa o indutor não,de +-5V no caso, não é utilizada nos calculos, pois o que interessa é a frequência deste sinal.

### 3. Idem exemplo anterior assumindo que o componente é agora um capacitor de 2 Farads

### Solução:

>			Zc = 1/ ω.C
>			Zc = ½.3,14.100.2
>			Zc = 1/1256
>
>			Zc = 0,000796 ohms

---------------------------------------------------------


Além das caracterizações das impedância realizadas acima, os conceitos fisicos pertinentes explicam que `Zl` e `Zc` atuam de modos opostos um ao outro. Desta forma, qualquer circuito elétrico básico, isto é, contendo `R`, `L` e `C` deve ser estudado de modo vetorial utilizando-se a seguinte representação gráfica:

![gss](https://cloud.githubusercontent.com/assets/3441126/9205016/36a13748-4036-11e5-9a87-2158c2ff6c83.png)
**<p align="center">L = recebe o valor de ω.L</p>**
**<p align="center">C = recebe o valor de 1/ ω.C</p>**
**<p align="center">R = recebe o valor da resistência total</p>**

![index](https://cloud.githubusercontent.com/assets/3441126/9205022/38e593dc-4036-11e5-8caf-1c11c2553365.jpeg)
![index2](https://cloud.githubusercontent.com/assets/3441126/9205024/39f34422-4036-11e5-9320-4a666d20e13f.jpeg)


------------
> Aula: 24 de agosto

----------


## Equivalentes de Thevenin e de Norton

Na prática, para nós, os equivalentes de thevenin e Norton constituem procedimentos que visam facilitar resoluções que envolvam nós e malhas tais como nos tradicionais equacionamentos Kirchoff, já esplorados em outras diciplinas.

Desse modo, definimos:

 - **Equivalente de Thevenin**: Associação de uma fonte de tensão com um resistor em série, isto é:
 
![img1](https://cloud.githubusercontent.com/assets/3441126/9579825/b1e4146c-4fcb-11e5-9288-f4e86ab8491b.png)

 - **Equivalente de Norton**: Associação, em paralelo, de uma fonte de corrente com um resistor, isto é:

![img2](https://cloud.githubusercontent.com/assets/3441126/9579826/b333012a-4fcb-11e5-8019-b3d99b37dad9.png)


A teoria envolvendo os equivalente de thevenin e Norton garante que para todo thevenin existe um Norton eletricamente equivalente e vise versa. Nas conversões os resistores mantem os seus valores e as transições de tensão para a corrente e vise versa são reguladas pela lei de ohm.

Muito mais popular na prática é o uso de **fontes de tensão**, isto é, a fonte que fornece uma vontagem fixa independentemente da carga conectada a ela. Alternativamente, dizemos tratar da fonte na qual a resistencia da carga, isto é, o aparelho a ser alimentado é muito **maior** que a resistencia interna da fonte. **Fonte de corrente**, por outro lado, constitui um modelo mais comum na teoria do que na pratica, tratando-se do elemento que se auto-regula para fornecer uma corrente constante independentemente da carga conectada a ela, alternativamente, dizemos tratar-se da fonte na qual a resistencia da carga é muito **menor** do que a resistencia interna.

Diante do exposto, passamos a analisar alguns exemplos.

- **Exemplo**: Determine a corrente no resistor de 50 ohms no circuito abaixo.

![img3](https://cloud.githubusercontent.com/assets/3441126/9586505/9b252ec8-4ff3-11e5-9987-815cc66e0d4f.png)

- **solução**:  Exceto ao elemento ao qual indagamos alguma grandeza, no caso a corrente no resistor de 50 ohm, procederemos com conversões Thevenin-Norton, visando simplificar o circuito por meio de associações de resistores e/ou fontes. Procedemos como segue:

![img4](https://cloud.githubusercontent.com/assets/13787877/10100558/f85a5e3c-6368-11e5-8fce-66bac10588ad.png)

-------------------

- **Exemplo 2**: Determine a tensão e a corrente no resistor de 100 ohm do circuito abaixo.

![img5](https://cloud.githubusercontent.com/assets/3441126/9586589/1f60b586-4ff4-11e5-80a2-ff28e345b8d2.png)


-----

- **Exemplo 3**: Idem anterior, invertendo a polaridade da fonte de `30 v` e associando, em serie com a fonte de `5 v`, de modo contraposto, outra fonte de `5 V`

![img6](https://cloud.githubusercontent.com/assets/13787877/10100944/b354a4d4-636b-11e5-8a18-1a96582eb335.png)


> **OBS**: Em nenhum momento encontraremos 2 fontes de corrente em série, a não ser que ambas possuem o mesmo valor de corrente e o mesmo sentido de polariadade. Caso contrario teriamos uma situação fisica impossivel, pois se a fonte de corrente mantem a corrente constante e a corrente é a mesma para todos os elementos de uma associação em serie, não podemos admitir situação divergente. Por outro lado, são admissiveis fontes de tensão em paralelo, situação na qual a tensão equivalente é a da maior das fontes e a corrente equivalente é a soma das correntes individuais. As polaridades dessas fontes de tensão não devem entretanto, ser contrapostas.

> **OBS**: Toda a teoria que envolve os equivalentes Thevenin e Norton pode tambem ser utilizada quando as fontes de alimentação existentes sob o circuito sobre analise forem alternadas. Nesse caso, costumamos utilizar como simbolos representantes das fontes de tensão correntes alternadas respectivamente:

![img7_](https://cloud.githubusercontent.com/assets/13787877/10101519/9c8ab348-636f-11e5-8462-ba0696c483cd.png)

> Alem de considerarmos os elementos `R`, `L` e `C` com as impedancias complexas já estudadas. Neste ambito as fontes são tambem tratadas em uma abordagem vetorial, constumeiramente conhecida como fasores e tensão em corrente 

-----

## Diodos semicondutores e aplicações

Conforme ja vimos anteriormente, os diodos constituem componentes que permitem a passagem da corrente eletrica apenas em um sentido, impedindo o fluxo de eletrons no sentido oposto desde que seja respeitado o limite maximo de tensão aplicada ao componente, pois, uma vez ultrapaçado o limiar, o diodo pode entrar em curto-circuito, permitindo a passagem da corrente em ambos os sentidos ou abrir-se, tornando-se um isolante. Fabricado com base nos materiais semicondutores silicio ou germanio, possui como simbolo eletrico:

![img8](https://cloud.githubusercontent.com/assets/13787877/10101577/eafe5d72-636f-11e5-989a-71d3bd762256.png)

Sendo `A` e `K`, respectivamente, os terminais anodo e catodo, ou seja, o que deve ficar com potencial mais positivo e mais negativo respectivamente, de modo a permitir a passagem da corrente eletrica, situação na qual dizemos que o componente está diretamente polarizado. Ligado ao contrario, dizemos que esta reversamente polarizado.

Não esquecemos que o diodo, para funcionarem, como comentado, possuem uma junção de dois micro cristais de silicio ou germanio, sendo que um deles é dopado com material do tipo `N` isto é, que possui cinco eletrons livres na banda de valencia e o outro é dopado com um material do tipo `P`, isto é, que possui tres eletrons livres na banda de valencia. As dopagens constituem a mistura de impurezas que penetram na estrutura atomica dos cristais de silicio ou germanio, alterando as suas propriedades fisico quimicas.

Um fato relevante que envolve o uso de diodos é que, estando diretamente polarizado, isto é, permitindo a passagem da corrente eletrica, o diodo força uma queda de tensão que é percebida mesmo sem fluxo de corrente, queda esta que está em torno de 0.6 a 0.7 `v` nos diodos de silicio e 0.1 a 0.2 `v` nos diodos de germanio. Este comportamento se distingue daquele ocorrido com materiais condutores, tais como os que compoe os resistores. Nestes, a falta de fluxo de eletrons, isto é, corrente eletrica nula, implica em manutenção da tensão da fonte 

![img9](https://cloud.githubusercontent.com/assets/13787877/10101762/f8206d14-6370-11e5-934d-8197fdca5210.png)

Percebe-se frequentemente a aplicação dos diodos em circuitos eletronicos tais como os de computadores, particularmente, nas fontes de alimentação. Presentes nos desktops e nos carregadores dos laptops os diodos possuem papel fundamental na conversão da tensão alternada da rede eletrica em tensão continua e de polaridade fixa necessaria para alimentar os componentes eletronicos dos circuitos computacionais.

Sabemos que a geração e transmição de energia eletrica entrega para os usuarios uma tensão alternada. Isto possibilita o uso de transformadores para reduzir 110v ou 220v para tensões aceitaveis pelos circuitos eletronicos computacionais, pois os transformadores somente funcionam com tensão alternada devido a variação do fluxo eletro magnetico que ela proporciona e, por outro lado, divisores de tensão resistivos não são convenientes para efetuar este tipo de redução, tendo em vista o aquecimento demasiado  ou a indisponibilidade de corrente eletrica. 

De qualquer forma, as tensões reduzidas com o uso de transformadores continuam sendo alternadas e os circuitos eletronicos computacionais somente aceitam tensões continuas. A conversão das tensões alternadas para continuas constituem um processo conhecido como **retificação** e que pode ser realizado utilizando-se diodos.

![img10](https://cloud.githubusercontent.com/assets/13787877/10101861/931ccc40-6371-11e5-9ee4-a15155ab4701.png)
![img10b](https://cloud.githubusercontent.com/assets/13787877/10102017/a881307a-6372-11e5-924f-86b169f15776.png)
A conversão da tensão alternada em tensão continua, realizada conforme o circuito que segue, com um unico diodo, é conhecida como retificação de meia-onda.

![img11](https://cloud.githubusercontent.com/assets/13787877/10102679/2d6d3ee8-6376-11e5-8f5b-8f33f336a111.png)
A saída está mais próxima do ideal, mas ainda existem flutuações, pois metade de cada período senoidal é periodo

Uma variação da retificação em meia onda é a retificação em onda completa que se faz com base em dois diodos, e é possivel quando o secundario do transformador possui uma derivação central, que é utilizada como terra, ou referencia. O efeito entretanto é o mesmo do circuito anterior. O esquema eletrico segue:

![img12_](https://cloud.githubusercontent.com/assets/13787877/10102899/7176f77c-6377-11e5-8c76-631cc428a070.png) 

A terceira tecnica de retificação, que é a mais propicea e mais utilizada industrialmente, utiliza 4 diodos e é conhecida como retificação em ponte, estabelencendo-se conforme o circuito abaixo.

![img13_](https://cloud.githubusercontent.com/assets/13787877/10103294/71840e4c-6379-11e5-90a1-61ffb63a9a31.png)


-----------

#### MINIPROVA 2

 -  Elabore, ao seu gosto, um circuito eletrico com 2 malhas e 2 fontes de alimentação de tensão continua, sendo uma em cada malha, com um unico resistor na intersecção das malhas. Enconte a corrente nesse resistor utilizando os equivalente de thevenin e norton e, em seguida, recorde os seus estudos anteriores e confira o resultado utilizando os leis de kirchoff por meio da resolução de um sistema 2x2.
 
--------------


Além dos circuitos de retificação observados anteriormente, destacamos a utilidade dos diodos semicondutores no sentido de proteger equipamentos contra possíveis inversões de polaridade das fontes de alimentação. A ligação no carregador do labtop constitui um classico exemplo. Nos laptops mais comuns, o plug que conecta o carregador ao computador é do tipo **P2** ou similar. Este plug por si só, ja impede inversões de polaridade, pois não há como conecta-lo erroneamente, entretanto,  no caso da eventual quebra do cabo, e posterior conserto, pode haver descuito e inversão dos fios, nesse caso, um diodo semicondutor poderia ser utilizado para evitar que a corrente eletrica tende circular pelo circuito com a polaridade indevida, danificando-o.

![img14](https://cloud.githubusercontent.com/assets/13787877/10103743/28631854-637c-11e5-9546-a1a81b450c99.png)

Notamos que o circuito acima não será danificado no caso de uma inversão de polaridade, devido ao diodo de proteção. Entretanto, com a polaridade invertida o circuito não funcionará. Podemos fazer uso de uma outra estrategia, comunmente utilizada nos macbooks da apple, para permitir que o circuito do labtop funcione normalmente indepemdente da polaridade em que a fonte é conectada.

Podemos utilizar uma ponte de diodos, aproveitando a ideia da retificação em ponte, estudada anteriormente, para alimentar o circuito na polaridade correta, qualquer que seja a polaridade da conexão da fonte.

![img15](https://cloud.githubusercontent.com/assets/13787877/10103884/d68e9944-637c-11e5-9c1e-13d801721411.png)


Interessantemente, percebemos que o uso da ponte de diodos na entrada dos laptops está restrito, atualmente, as maquinas da apple. Tal fato é devido, principalmente, ao custo, não dos diodos, mas sim dos componentes existentes dentro do carregador, pois este deverá fornecer quase `1,5v` a mais do que forneceria caso a ponte de diodos não existisse. circuitos tais como retificadores normalmente necessitar manter correntes consideraveis, e portanto o silicio deve ser adotado ao invez do germanio, implicando em queda de aproximadamente 0,7v por diodo. Tendo em vista que este modelo de retificador requer que a corrente circule por 2 diodos, justificamos os comentarios.


Diodos são também comunmente utilizado em circuitos computacionais na confecção de memórias programadas em nível de hardware e com uma gravação única definida pelo fabricante. Por meio da propriedade de somente permitir a passagem da corrente elétrica em um único sentido, são aproveitados para definir estruturas de memória conhecidas como **matrizes de diodos**. Constituem configurações tais como a que segue:

![img16](https://cloud.githubusercontent.com/assets/13787877/10104333/98cbb260-637f-11e5-8222-89fda63e76fa.png)


No circuito acima, o funcionamente básico ocorre em virtude do posicionamento dos diodos. Para ler dados da saída, basta conecta-la as entradas do circuito que irá receber os códigos gravados, que normalmente corresponde as entradas de algumas portas lógicas. Para que as saídas apresentem os códigos gravados em cada um dos endereços basta alimentar, com uma fonte de tensão, o endereço desejado, sendo que somente um endereço pode ser alimentado por vez. Tendo em vista a considerável sensibilidade das portas lógicas que receberão os sinasi de saída, nenhuma dessas linhas elétricas pode ficar desconectada de um nivel estabelecido de tensão, isto é, elas não podem "flutuar". Para isso a solução comunmente adotada é a ligação, em cada linha de saída, de um resistor de alto valor ao negativo de alimentação("terra"). Tais resistores, chamados de pull down, garantem que se não ouver nivel lógico 1 em determinada saída, ela estará fisicamente, ainda que passando pelo resistor, conectada ao nivel lógico 0, por outro lado, quando o nivel logico 1 estiver presente, os resistores em nada atrapalharão, pois desviam uma parcela infinea da corrente elétrica para o terra.

 - **Exercicio**: Elabore uma memória baseada em matriz de diodos, contanto com os resistores de pulldown, que possibilite, em sua saida de 4 bits, a leitura de todos os valores binarios inteiros, entre 0 e 15, cada qual acessivel por meio de um endereço. Assim, no endereço `E0` deve estar gravado o valor 0, e assim por diante até o `E15`.

![img 17](https://cloud.githubusercontent.com/assets/3441126/9581037/6a4cd672-4fd3-11e5-96e3-71ea50d59cf8.png)

**<p align="center"> Continua ...</p>**


> Um tipo particularmente importante de diodo é o tradicional **light-emittind diode(LED)**. Este componente, disponivel comercialmente em varios formatos, tamanhos e cores, possui em sua composição, alem dos cristais de silicio, dopados com materiais P e N, outro elemento químico para a liberação dos photons da junção dos 2 cristais. Este elemento normalmente é o arceneto de galium (AsGa). É muito importante observar que todo LED, para qual o simbolo é um diodo com duas setas apontando para fora, requer normalmente um resistor em série com ele em qualquer um dos terminais para emitir luz na intensidade conveniente e sem ser danificado, conforme o circuito abaixo:

> ![img 16](https://cloud.githubusercontent.com/assets/3441126/9587100/0d8ed1be-4ff7-11e5-9b17-a095853a33cc.png)


> Para determinar o valor de R ideal, para trabalhar em conjunto com o LED, devemos recorrer ao manual do fabricante do LED para descobrir qual é a corrente que deve passar por ele para mante-lo iluminado sem que ele se danifique. Na prática, não recorremos, entretanto, aos manuais, pois em geral os LEDs trabalham idealmente com correntes entre 10 e 20 miliamperes. Desse modo determinamos `R` em função desse dado.

> - Exemplo: Determine `R` no circuito acima considerando que a fonte é de 12v.

> - Solução:
>    U=RI
>    R=U/I =  12-0.7/0.0113 (queda de tensao diodo(queda zener))
>    11.3/0.0113 = 1000 ohm

----------------

### MINIPROVA 3
 - Explique as diferenças existentes entre a retificação de meia onda e a retificação em ponte, comentando caracteristicas vantagens e desvantagens.

---------------

## Diodos Especiais

Algumas modificações nas estruturas fisico-quimicas durante a construção dos diodos retificadores comuns, particularmente utilizando silicio ao invez de germanio, permite obter diodos que possuem comportamentos eletricos distintos dos tradicionais. Um tipo especial de diodo é conhecido como **zener** e possui o seguinte simbolo eletrico:

![img18](https://cloud.githubusercontent.com/assets/13787877/10104481/38dbcf56-6380-11e5-9253-bc70b82bcbc4.png)

Este diodo, quando diretamente polarizado, conduz normalmente a corrente elétrica, assim como o diodo retificador comum. Por outro lado, quando inversamente polarizado, isto é, quando ligado no sentido contrario de condução, pode tambem conduzir a corrente em proporções variaveis, de modo a fazer com que a tensão em seus terminais seja constante, mesmo mediante variações da tensão de entrada no arranjo divisor de tensão composto de um resistor e o diodo zener. Desse modo, o diodo zener funciona como um elemento estabilizador, isto é, regulador de tensão, conforme exemplificado a seguir:

![img19](https://cloud.githubusercontent.com/assets/13787877/10104584/ccba5cce-6380-11e5-92ec-8bf10f3f1cd0.png)


Os diodos zener não possuem valores ou código de cores. Ao contrario, eles possuem uma sigla que, de acordo com o manual do fabricante, especifica as suas caracteristicas comportamentais. Os principais parametros são a tensão de estabilização a tensão maxima de entrada, e a corrente, ou potencia, maxima que ele suporta. É ainda importante observar os calculos necessarios para determinar o valor mais ou menos propíceo do resistor que se associa ao zener na tabela de regulagem, tal como no circuito acima.

Nesse circuito acima, imaginando que o circuito a ser alimentado com a tensão regulada de `5V` consuma uma corrente de `0.1A`. Desse modo temos:

>`U = (R+r)I`
>
>`U = 12`
>
>`I = 0,1`
>
>`R+r = 12/0,1 => R+r = 120 ohms`
>
>`U=rI`
>
>`5=r.0,1`
>
>`r=5/0,1`
>
>`r = 50 ohms`
>
>`R+r = 120`
>
>`R = 120-r => R = 70ohms`



Alem disso, a potencia dissipada pelo zener e pelo resistor `R` podem ser calculadas.

**<p align="center"> P = U . I</p>**

Para o zener, temos `5V . 0.1A = 0.5W` , alem disso, para o resistor `R` temos ` 7V . 0.1 = 0.7W`.
Resumindo, a compra dos componentes para este circuito corresponde a:

 - 1 diodo zener para `5V` e `0.5W`
 - 1 resistor de `70ohm` para `0.7W`

Neste circuito em especifico é importante informar, no momento da compra, as potencias, pois, caso contrario, principamente no caso do resistor, a falta de especificação implicará na venda de componentes padrão, isto é, de um quarto ou oitavo de `w`, que neste caso, não suportariam o aquecimento. Finalmente lembramos que não são todos os possiveis valores de resistores que existem no comercio. No caso, `70 ohm` não é um valor comercial, sendo, `68 ohm` o valor comercial mais proximo. Para nós, este valor é adequado, pois o zener se auto-ajustará para balancear a diferença.

-----------

 - Exercicio: Projete um circuito estabilizador de tensão, com divisor de tensão por zener, que receba na entrada, tensão em torno de `9 v` para alimentar um processador com `3.3 V` e que consuma uma corrente maxima de `0.2 A`. Especifique os detalhes do zener e do resistor conjugado com base nas referidas caracteristicas.
 

![img21](https://cloud.githubusercontent.com/assets/13787877/10104897/6859c8ee-6382-11e5-8632-829a6035ce58.png)

Desse modo, o resistor `R` será de `28.5 ohm` por `1.14 W`. Comercialmente, os valores mais proximos disponíveis são: `27 ohm` e `2 W`. O zener por sua vez será de `3.3 V` por `0.66 W`. Comercialmente os valores mais proximos são: `3.3 V` por `1 W`.

-----------

Um outro tipo de diodo especial é conhecido como **diodo Varicap** que possui o seguinte simbolo elétrico:

![img22](https://cloud.githubusercontent.com/assets/13787877/10104946/ae0d8628-6382-11e5-876c-d825ff013959.png)

Este componente, quando diretamente polarizado, funciona como um diodo comum retificador. Por outro lado, quando inversamente polarizado, ele tambem funciona como um diodo retificador comum, mas com a particular propriedade de atuar como um capacitor, para qual a capacitancia depende da tensão que chega aos seus terminais. Na pratica, este componente é utilizado para substituir capacitores variaveis, que são muitas vezes mecanicamnete inviaveis. Desse modo, podemos controlar uma capacitancia com base em tensão, e não diretamente com base em ajuste mecanico.

Injetando tensão no diodo inversamente polarizado, a agromeração dos portadores de carga em ambos os cristais de slicio dopados se aglomeram, simulando duas placas condutoras separadas por um isolante, trazendo assim o efeito capacitivo. Um caso classico de aplicação é o do circuito abaixo.

![img23](https://cloud.githubusercontent.com/assets/13787877/10119174/d0d00964-6464-11e5-85c0-7d9534843583.png)



--------------

## ARTIGO 1:

Confeccionar um pequeno texto em latex e em ingles com no maximo 3 paginas, opcionalmente contendo figuras e tabelas, com formato livre, mas contendo ao menos:

 - Abstract
 - Discusão
 - Referencias (3 ou 4 bastam)

Com o tema ** A tecnologia de fabricação de circuitos integrados: Complementary Metal-oxide semiconductor (CMOS)**

-------

## Mini Prova 4
 - Assumindo uma fonte de tensão continua, mas ajustável entre 10 e 20 volts, projete um pequeno circuito com zener para, mediante qualquer entrada de tensão na faixa mensionada, entregar na saida 6 volts, com capacidade para 50 miliamperes. Forneça as especificações completas do divisor de tensão formado pelo resistor e pelo zener.

-------------

## Osciladores e Cristrais

Na eletrónica, inclusive nos circuitos computacionais, o componente conhecido como **cristal de quartzo** consiste de um elemento que possui extrema estabilidade para controlar frequencias de ressonancia, ou frequencias de vibração. Particularmente, os circuitos conhecidos como **osciladores** são aqueles que produzem vibrações, em nosso caso, vibrações eletricas, caracterizadas por variações periódicas de tensão ao longo do tempo, comumente expressas em modo gráfico por meio de ondas, tais como a onda **quadrada**, **retangular**, **senoidal**, **triangular**, entre outra.


![wavetypes](https://cloud.githubusercontent.com/assets/3441126/9992658/e252a90e-6049-11e5-97d0-202444fd5b74.gif)


Eletricamente, o ocilador é um amplificador no qual parte do sinal de saida retorna à entrada, estabelecendo assim, um **ciclo**. Existem diversas formas de controlar como a parcela que retorna à entrada se comporta, o que influencia diretamente na frequencia e na amplitude do sinal alternado do ocilador. Resistores, capacitores e indutores são opções para o controle deste retorno, e portanto, da frequencia de ocilação. Tais componetes, entre tanto, possui caracteristicas fisicas que facilmente se alteram em função da temperatura, pressão, umidade do ambiente, entre outros fatores. **O cristal de quartzo**, por outro lado, é, conforme mencionado, **extremamente estável**, quase não sofrendo a influencia de fatores externos. A sua frequencia de resonancia é dada por suas dimensões fisicas e pelo modo como ele é cortado, ou lapidado industrialmente. Particularmente, dizemos que o quartzo é um cristal, ou material, **piezoelétrico**, isto é, vibra mediante um esforço mecanico ou elétrico aplicado em seus terminais.

Um exemplo segue:

![img25](https://cloud.githubusercontent.com/assets/13787877/10136599/a2a12e5c-65cb-11e5-958d-577e066ef5cb.png)

No circuito acima, o simbolo **-| D |-** representa o cristal de quartzo. Observamos que, por meio de um resistor, parte da tensão presente na saida da porta lógica retorna a sua entrada via resistor. Este retorno é a condição que comentamos inicialmente para a manutenção da oscilação. Alem disso, o resistor alimenta o cristal, cauzando nele, uma pressão elétrica, o que faz com que ele vibre na frequencia para a qual ele foi cortado, ou lapidado. Desse modo, por exemplo, se requisitamos na industria eletrónica o corte de um cristal para 7mhz, por exemplo, e utilizamos ele no circuito acima, então obteremos na saida da porta logica, esta mesma frequencia.

Uma particularidade interessante é o simbolo:

![img26](https://cloud.githubusercontent.com/assets/13787877/10105424/f98833b2-6384-11e5-94e3-aeafabadc943.png)

que esta inserido dentro da porta lógica, ele significa que a porta lógica não é comum, mas sim do tipo **gatilho de Smith** (Smith Trigger). Isso significa que esta porta lógica defini muito bem as transições entre `0` e `1`, correndo pouco ou nenhum risco de ficar "confusa" com variações suaves presentes na sua entrada. Por isso, este tipo de porta é normalmente utilizada em osciladores para os quais a intenção é obter na saida uma forma de onda quadrada. 

O controle dos processadores é uma das aplicações que depende dos cristais de quartzo, pois é sempre necessario haver um oscilador extremamente preciso que controla a frequencia do seu funcionamento, isto é, o tempo do ciclo de maquina. Normalmente um ciclo de maquina ocorre a cada borda de subida, ou borda de descida, da onda quadrada o ocilador. Os conversores analogico para digital tambem constituem circuitos computacionais e dependem da precisão proporcionada pelos cristais, pois sabemos que o precessamento de um tipo qualquer de sinal analogico em um computador está baseado no **teorema da amostragem**.

Assim, por exemplo, tratar computacionalmente um sinal acustico musical, implica normalmente em fazer com que o conversor A/D  trabalhe na taixa de 44.100 amostras por segundo, pois o ouvido humano somente percebe frequencias até o limite de 22.050 hz. Um oscilador preciso naquela frequencia, é por portanto necessario, para fazer com que o conversor A/D capture uma amostra a cada 1/44100 segundos, sendo que as capturas toda vez que haver uma borda de subida ou descida (conforme o projeto).

![img27](https://cloud.githubusercontent.com/assets/13787877/10118897/95abf6c6-645b-11e5-9417-5a1fbfdf08d2.png)


 - OBS 

Algumas vezes é necessario realizar um pequeno ajuste na frequencia de vibração de um oscilador à cristal. Em principio, só poderiamos fazer isso industrialmente, alterando as dimenções e o formato do cristal. Este processo, entretanto, pode ser impraticável, principalmente, se o ajuste pretendido é algo, por exemplo, fazer com que o cristal industrializado para vibrar em 30 MHz passe a vibrar em 29.999 ou 30.0001 MHz. Uma possibilidade alternativa para realizar este ajuste, sem alterar fisicamente o cristal, é, conforme percebido e comprovado por fisicos e engenheiros, adicionar uma capacitancia em serie com o cristal isto é

![img28](https://cloud.githubusercontent.com/assets/13787877/10118901/d07d3c4c-645b-11e5-9063-389b7c0db649.png)

Conforme o valor do capacitor dar se a maior ou menor nivel de variação em sua frequencia, mas obviamente dentro de uma minima faixa, assim por exempo, um oscilador variavel na faixa de 29.999 até 30.0001 pode ser obtido utilizando um capacitor ajustável, ou variavel, em serie com o cristal

![img29](https://cloud.githubusercontent.com/assets/13787877/10118962/3384bf70-645e-11e5-9a72-8546e89e74f5.png)


Tendo em vista que o trimmer é normalmente muito pequeno e requer chaves de fenda para o seu ajuste e que o capacitor variável é muito grande e caro, é comum utilizar, em serie com os cristais um terceiro componente elétricamente equivalente e que possui a sua capacitancia variavel em função da tensão continua que nele chega. Este componente, conforme ja comentamos, o **diodo varicap**. Nesse caso, o arranjo circuital típico é normalmente similar ao exposto a seguir

![img30](https://cloud.githubusercontent.com/assets/13787877/10119101/e149b094-6462-11e5-95da-ccfb84331c89.png)


----------------

### Observação:

Em meados da decada passada, a industria de computadores passou a utilizar com mais frequencia duas tecnicas de soldagem:

 - Surface Mount Device (SMD)

 - Ball Grid Array (BGA)

Desenvolvendo inclusive estações de solda propiceas para cada uma das respectivas tecnicas. Basicamente, na primeira, os componentes eletronicos possuiem os terminais bem proximos um dos outros e bem curtos, pois a fixação mecania e a soldagem ocorem do mesmo lado da placa de circuito impresso. No segundo modelo além da fixação mecanica e da soldagem serem efetuadas do mesmo lado da placa, os componentes eletronicos são fabricados de modo que os seus terminais sejam na verdade micro bolas de cobre localizadas em baixo do componente 

### MiniProva 5

 - Discuta prevemente as diferenças dos padrões SMD e BGA de soldagem, tentando justificar o porque do uso deles, principalmente o segundo, pela industria de computação. Inclua comentarios sobre o maquinario necessario para produzir soldas em cada uma das tecnicas e uma figura relacionada com cada uma das tecnicas.


------------
> Aula: 28 de setembro

----------

### Comentários sobre resistores especiais:

Com base nos estudos realizados anteriormente, é de interesse mencionarmos alguns tipos de resistores classificados como especiais. Entre eles temos:
- **Light Dependent Resistors (LDRs)**:
São resistores dopados com um material que os torna sensíveis a luz, de modo que, quanto mais luz incidir na sua superfície, menor a sua resistência Ohmica. O material utilizado é normalmente, sulfeto de cadmio. E o símbolo elétrico é o seguinte:
![img31](https://cloud.githubusercontent.com/assets/13787877/10137368/8541f860-65cf-11e5-81d8-0323994a3685.png)

Esse resistor é normalmente utilizado em circuitos mais gerais, tais como, aqueles que comandam o acendimento automático de lâmpadas em residências e postes de iluminação, assim como nos mais específicos, tais como controles remotos, mouses ópticos e leitores de cd/dvd. Em geral o LDR é utilizado em conjunto com outro resistor, na configuração de divisor de tensão, tal como no exemplo a seguir: 
![img32](https://cloud.githubusercontent.com/assets/13787877/10137542/6ce6eb58-65d0-11e5-995c-d95785243325.png)

O LDR é um componente, normalmente, com dimensões mínimas, da proporção de um grão de feijão ou menor e que não possui códigos de cores ou valores impressos. Ao contrário, possui apenas um código, pelo qual podemos encontrar no manual do fabricante as suas características, tal como a faixa de variação da resistência em função da intensidade da luz incidente.

- **Termistor**: Trata-se de um componente que varia o valor da sua resistência Ôhmica em função da temperatura que é recebida em seu corpo. Pode ser do tipo Negative Temperature Coeficient (NTC) ou Positive Temperature Coeficient (PTC) nos quais, a resistência diminui ou aumenta respectivamente em função do decaimento da temperatura. Em âmbito geral é um componente que pode ser utilizado em termômetros digitais. No âmbito computacional costuma ser utilizado para controlar o ligamento, desligamento e velocidade do cooler do computador frente ao aquecimento do processador. O seu símbolo elétrico:
![img33](https://cloud.githubusercontent.com/assets/13787877/10137606/b66ceb1a-65d0-11e5-9891-a6cbe649f12e.png)

E a configuração circuital típica, na qual ele é utilizado, é normalmente similar a configuração usada para o LDR.

- **Extensômetro**: Trata-se de um resistor, também conhecido como: strain-gauge, para qual o valor da resistência ôhmica varia em função da deformação mecânica em que o componente sofre. Em geral, do ponto de vista físico, o componente é tal qual uma pequena fita ou um pequeno adesivo que é colado em um material que sofre deformações. Normalmente, utiliza-se o extensômetro simbolizado como um resistor comum, para relacionar o ângulo de deformação com uma determinada resistência ôhmica. O seu uso mais comum é na área de automação, mas em alguns laptops têm sido utilizado no controle da iluminação da tela frente a abertura ou fechamento do aparelho.

--------------------------

> Aula 19/10/15

-----------------------------

## Transistores

São componentes considerados **ativos** na eletrónica, isto é, requerem alimentação para desempenharem as suas funções em um circuito. Desse modo, além de necessitarem de entradas e produzirem saídas em função de uma tensão em circuitos analógicos ou digitais, requerem também uma fonte de alimentação. Essa característica confronta com os componentes anteriormente estudados, que são considerados passivos, isto é, transformam de algum modo uma tensão que lhes é aplicada sem necessitarem de uma fonte de alimentação para tal. Os transistores, que surgiram com base nas pesquisas realizadas por físicos do **Bell Labs** nos Estados Unidos, tem proporcionado desde a década de 50 o avanço nos circuitos chamados computacionais, permitindo praticamente a substituição completa das valvulas eletrónicas, que são muito maiores e dicipam muito mais energia. Atualmente, o espaço fisico ocupado por uma valvula eletrônica é sulficiente para abrigar trilhões de transistores. Os transistores possuem a funcão basica de amplificar sinais elétricos analógicos ou digitais, assim como funcionar como chave eletrónica, isto é produzir ou não uma tensão na saida mediante as carateristicas de um sinal de entrada. No hardware computacional, a segunda função é a mais comum. fisicamente, os transistores são constituidos por duas junções de materiais semicondutores dopados, tal como ocorre com os diodos. Uma analogia comunmente utilizada é a seguinte:

![2 diodos ser](https://cloud.githubusercontent.com/assets/3441126/10577784/97797f70-764c-11e5-8d48-6fe19a45b20f.png)

Na figura acima temos 2 diodos contrapostos em série, dos quais ja sabemos que são formados por materias N e P, fazendo com que a corrente elétrica possa circular somente em um sentido. No ponto central da associação serie temos ainda uma derivação. Isso dá origem a um componente de 3 terminais que são chamados coletor(C), base(B) e emissor(E). A figura acima constitui de fato apenas uma analogia, pois nela observamos que a quantidade de material do tipo P é maior do que cada um dos cristais de material N, isto é, :

![captura de tela de 2015-10-19 09 49 37](https://cloud.githubusercontent.com/assets/3441126/10578426/d305329c-7650-11e5-8aad-d494f23a7c31.png)


Facilmente percebemos, com o nosso conhecimente anterior sobre diodos, que não é possivel obter fluxo de elétrons, isto é, corrente eletrica, entre os terminais **C** e **E** pois os diodos estão contrapostos. Seria apenas possivel obter fluxo de corrente entre os terminais **B** e **E** em um sentido e entre os terminas **C** e **E** em outros. Os fisicos do Bell Labs descobriram que se alterarmos a estrutura cristalina da figura anterior de modo a reduzir consideravelmente a espessura do cristal central do material P de modo que ele seja muito mais fino do que os de material N, e, alem disso, aplicarmos uma pequena redução na espessura do cristal N ligado ao terminal E, ou seja, se tivermos algo do tipo :

![captura de tela de 2015-10-19 09 56 59](https://cloud.githubusercontent.com/assets/3441126/10578440/ebbb0ec4-7650-11e5-887a-11efd4d8d3c3.png)


Teremos contruido um transistor

Particularmente, este transistor acima é conhecido como transistor do tipo **NPN**, pois existe um cristla do tipo P em meio a dois do tipo N. O simbolo elétrico desse componente é o seguinte:


![captura de tela de 2015-10-19 09 58 05](https://cloud.githubusercontent.com/assets/3441126/10578454/fdaee66e-7650-11e5-88af-cbfd02e8f093.png)



Alguns autores preferem utilizar um segundo simbolo que consiste no anterior inserido em um circulo, isto é, 

![transistor-npn_1](https://cloud.githubusercontent.com/assets/3441126/10578719/9d6f0890-7652-11e5-9878-60d9bfee17e9.png)


Para esse componente, com as condições retroespecificadas com as estruturas das cristais o funcionamento é o seguinte:

- Mediante uma corrente relativamente pequena,que venha a circular entre os terminais base e emissor, obedecendo o sentido correto da polarização, isto é, o lado mais positivo na base e o mais negativo no emissor, uma consideravel corrente passa a circular entre os terminais coletor e emissor, injetando a parte mais positiva no coletor e a mais negativa no emissor. Isso ocorre apesar da aparente polarização incorreta entre coletor e emissor.

Diante do exposto, temos o seguinte circuito típico para utilizar um transistor NPN como amplificador 

![ex_trnasistor](https://cloud.githubusercontent.com/assets/3441126/10578614/ec310aba-7651-11e5-8adc-43364f592a77.png)


No circuito acima, a corrente elétrica que circula entre a base e o emissor do transistor, com o auxilio da resistencia ohm muito grande, é conhecida como **corrente de base** (`Ib`). Por outro lado, a corrente elétrica que circula entre o coletor e o emissor do transistor, mediante comutação pela corrente de base, é conhecida como corrente de coletor (`Ic`). Assim podemos ainda definir uma terceira corrente que é a de emissor (`Ie`) sendo que `Ie = Ib + Ic`

![fig10](https://cloud.githubusercontent.com/assets/13787877/10579309/1b6021be-7656-11e5-99be-0415f145c209.png)

Devemos notar que em relação a **Ic**, Ib é muito pequena e portanto, na pratica, Ic e Ie são quase iguais, sendo na verdade Ie apenas ligeiramente mais que Ic. Devemos ainda notar que os transistors não possuem valores ou codigos de cores. Ao contrário, são como os diodos, isto é, possuem um código do fabricante que possibilita a consulta a um manual que contem as suas especificações e os seus principais parâmetros, que são os seguintes:

 - **Ic max**: corrente máxima de coletor suportada pelo componente;
 - **Ib max**: corrente máxima de base tolerável;
 - **B (beta)** : trata-se do parametro beta, que é o parametro mais importante, correspondendo ao seu fator de aplificação, sendo válida a relação **Ic = B Ib**. 

Devemos notar que B é uma propriedade intrisseca, isto é, inerente ao transistor e não pode ser alterada por compoentes externos. Comercialmente o valor de B para os diversos transistores existentes costuma variar desde de 50 até 1000 ou 10000. Observamos ainda que o parametro B na verdade relada o potencial maximo de amplificação, pois a corrente de coletor que está em sua função não atinge necessariamente o valor **B.Ib**. De modo geral, a amplificação ocorre de forma linear (ou quase) até um certo ponto em que o aumento da causa(Ib) não proporciona mais aumento do efeito(Ic), sendo esse ponto conhecido como **ponto de saturação**.

![grafico1](https://cloud.githubusercontent.com/assets/13787877/10579310/1b5fa040-7656-11e5-8c39-587bbf1e649f.png)



O manual do fabricante descreve para cada transistor, alem dos parametros acima, observações relativas ao encapsulamento, pois os tres terminais (base, coletor e emissor) não obedecem, em termos de posicionamento fisico, nenhum padrão especifico, variando de transistor para transistor. Os encapsulamentos mais comuns são aqueles dos transistores BC338, BD139, TIP31, ZN2222 e MRF454. O primeiro é um transistor de baixa potencia, o segundo de média e o terceiro de alta potencia. O quarto possui capsulamento especifico para operar em altas frequencia, sendo comunmente utilizado em circuitos de radio transmissão. O Ultimo possui um encapsulamento relativamente maior que os demais, sendo comunmente utilizado em amplificadores de altissima potencia para radio transmissão. O segundo, o terceiro e o ultimo possui inclusive meios para fixação de dicipadores de calor.

Até o momento mencionamos um unico tipo de transistor, que é o NPN. É possivel entretanto construir transistores para os quais existe um cristal N entre 2 cristais P. De modo análogo temos:

![fig1](https://cloud.githubusercontent.com/assets/13787877/10728355/3c548988-7bc8-11e5-818e-68759a05227b.png)

O simbolo elétrico correspondente é:

![fig2](https://cloud.githubusercontent.com/assets/13787877/10728375/6c700912-7bc8-11e5-8480-bca948c85254.png)


NPN e PNP são portanto os dois tipos de transistores conhecidos como ***bipolares**, que são os mais comuns. Transistores especiais serão descritos adiantes. É importante ainda lembrar que no caso do transistor PNP, as polaridades das pontes indicadas nos circuitos anteriores devem ser invertidas pois os diodos internos ao transistor estão invertidos.

Com relação as configurações circuitais para o uso dos transistores, existem 3 possibilidades:

 - Emissor-comum, base-comum e coletor-comum, nas quais a palavra comum significa que o respectivo terminal serve quanto a entrada quanto a saida. Assim, os exemplos anteriores estão na configuração emissor comum, sendo que as outras 2 possuem uso mais especifico e fora do escopo deste curso.

----------

### Miniprova 6
 - Descrever brevemente o que é e como funciona o modelo Ebers-Moll de funcionamento do transistor bipolar.

-------------


 - **Obs**

Comercialmente, existe uma configuração especifica em que 2 transistores são conectados de modo que o seu potencial de amplificação é tal que ambos os componentes são vistos como um unico transitor em que o fator de amplificação **B** corresponde a multiplicação dos **B** individuais. Este "super transistor" é conhecido como transistor de configuração **Darlington**. Um exemplos classico disponivel no mercado é o **BC517**, este componente é muito comum na configuração de emissor comum o ganho ser tão alto que aproximando a mão do terminal base em aberto, ja passa a haver condução entre o coletor e o emissor. Particularmente, além de ser possivel adiquirir no comercio transistores do tipo darlington, podemos produzi-los com dois transistores tradicionais. A configuração é sempre a seguinte:

> img 2 transistor em serie


--------

## Tansistores especiais 

Os circuitos computacionais, na maioria das vezes, não são construidos simplemente com transistores bipolares. Após a invenção dos mesmos, na decada de 50, outros estudos foram iniciados no sentido de melhorar a proposta de fazer com que uma força menor pudesse acionar, ou controlar, uma forma maior. Além disso, questoes relativas ao consumo de energia e, consequentemente a dessipação de calor, passavam a ser preocupações releantes. Surgiu então, tempos após o lançamento comercial do transistor bipolar, uma outro tipo de transistor conhecido como **transistor de efeito de campo (FET - field effect transistor)**. Neste componente a ideia é que um campo elétrico pudesse acionar e controlar uma energia de grande potencial. O campo elétrico mencionado permitiria assim um efeito que não traria a necessidade de um fluxo de eletrons, isto é, a corrente elétrica. Nesse sentido, o FET é conhecido na eletronica como amplificador de transcondutância, isto é, possui altissima impedancia de entrada, da ordem de centenas de melhares de ohm, e também alta impedancia de saída, de modo que podemos dizer que em sua entrada, o controle da amplificação é realisado por tensão e não por corrente, e a grandeza controlada se faz em termos de corrente.

Ao longo do tempo foram desenvolvidos os seguintes tipos de transistores **FET**:
 - J-FET ( junction FET): é o modelo mais simples do FET e que não é demasiadamente sensível à cargas estáticas. Assim como ocorre com os transistores bipolares NPN e PNP, os **J-FETS** também possuem dois tipos de montagem que variam as polaridades das fontes à eles conectadas, que são o J-FET canal N, e o J-FET canal P, sendo que o primeiro é muitissimo mais comum e seu símbolo elétrico é:  

![jfet-nch](https://cloud.githubusercontent.com/assets/3441126/10735675/5457e70a-7bf0-11e5-9fb6-a1dff84e7e7c.png)

O terminal **S** (source), ou fonte, é por onde os elétrons entram, o terminal **D** (drain), ou dreno, é por onde eles saem, e o terminal **G** (gate), ou porta, é o que controla o campo elétrico que permite a condução entre **D** e **S**.
 - MOS-FET (metal oxide semicondutor FET): trata-se de um componente muito mais sensível que o anterior, porém que pode mais facilmente ser danificado por cargas estáticas. Constitui o componente ativo básico da grande maioria dos circuitos digitais memórias e processadores da atualidade. A sua construção permite classificá-lo em dois subtipos que são D-MOS-FET (mos-FET de depleção) e E-MOS-FET (mos-FET de intensificaçã, o e vem de enhacement (intensificação). O primeiro subtipo tem o funcionamento de modo a permanecer normalmente fechado, ainda que parcialmente. Isso significa que mesmo sem a presença de qualquer campo elétrico oriundo de tensões no terminal **G** já existe um pequeno fluxo de corrente entre os terminais **D** e **S**, que aumenta a medida que a tensão em **G** aumenta. Por outro lado, o segundo subtipo permanece normalmente aberto, ou seja, a ausência total de tensão em **G** faz com que não exista passagem de elétrons entre **D** e **S**

=====
Falta a parte que os pcs ficou cagado
=====

Unijuncao

ASsim como os FETS especificado anteriormente, os transistores unijunção como o próprio nome diz, são formados por uma única junção de um material N com um material P, ambos silício dopado, com material N consideravelmente maior que o P. O seu princípio de funcionamento é bastante particular e difere do transistor bipolar no sentido de que quando passa a conduzir em virtude de alguma tensão aplicada em sua entrada, a condução é praticamente plena, não variando linearmente em função da entrada. Sua consituição física e símbola segue:

![unijuncao](https://cloud.githubusercontent.com/assets/3441126/10735704/722402a0-7bf0-11e5-9fe9-e8f86c1181ad.png)


====
Diodos especiais
====

## Silicon-controlled rectifier (SCR)
Trata-se de um componente com três junções semi-condutoras de quatro cristais de silício. Da seguinte forma: 

![pnpn](https://cloud.githubusercontent.com/assets/3441126/10735713/7d958df2-7bf0-11e5-9775-470b859dc604.png)


A sua constituição física faz com que o componente funcione como uma chave comutadora que uma vez acionada permanece ligada enquanto houver alimentação no circuito. O símbolo elétrico é o seguinte:

![src-simbolo](https://cloud.githubusercontent.com/assets/3441126/10735716/809882a2-7bf0-11e5-9c53-ba1e9776e0b3.png)

Sendo respectivamente, A, K, G os terminais designados ANODO, CATODO e GATE. Uma vez que o terminal G receba tensão maior ou igual que 0.6V ou 0.7V, passa a ocorrer um fluxo de elétrons entre A e K sendo A o lado mais positivo. Tipicamente o circuito abaixo é um dos que ilustra o seu funcionamento:

![circuito-scr](https://cloud.githubusercontent.com/assets/3441126/10735736/a5d3e124-7bf0-11e5-8959-ae8cd182a1d1.png)

## SCR de mão dupla (TRIAC)

O SCR, conforme especificado acima somente permite a passagem da corrente elétrica, mediante autorização em único sentido, isto é, terminal A deve estar conectado no positivo de alimentação. Isto implica que somente podemos comutar cargas alimentadas por corrente contínua. Se desejamos, por outro lado, acionar eletrodomésticos e aparelhos maiores, alimentados com corrente alternada, devemos utilizar o SCR de mão dupla, ou TRIAC, que é simbolizado da seguinte forma:


![triac-simbolo](https://cloud.githubusercontent.com/assets/3441126/10735747/b2a56a9e-7bf0-11e5-8d60-04686c0f4242.png)


Sendo G, T1 e T2 respectivamente, o GATE, o terminal de carga 1 e o terminal de carga 2. Visando proporcionar uma analogia de funcionamento com base em transistores, podemos estabelecer o seguinte circuito para o caso do SCR:

![circuito-simula-triac](https://cloud.githubusercontent.com/assets/3441126/10735750/b526b700-7bf0-11e5-884b-315f1901b738.png)

----------

### Mini Prova 7
 - Pesquisar na internet um circuito simples baseado em scr, copia-lo e comentar seu principio de funcionamento.
 
------------------


> Aula 09-11-2015

### Circuitos integrados amplificadores operacionais

Circuito integrado é o nome que se dá a um conjunto de componetes eletrònicos ativos e passivos devidamente conectados na forma de um circuito, sendo que o circuito em si é encapsulado em um único envolucro. Desse modo, observamos que um circuito integrado com volume de alguns milimetros cubicos pode conter trilhoes de componentes. Ja sabemos que transistor real, por exemplo, é muitissimo menor do que o transistor vendido comercioalmente, pois a sua capa plastica ocupa normalmente de 90 a 99 por cento do seu volume total. Isso acontece com grande parte dos compoentes eletronicos visando apenas possibilitar a sua minipulação mais confortavel. Daí entendemos por que um unico circuito integrado pode reunir tantos componentes. Se, por um lado, resistores, diodos e transistores podem ser facilmente inseridos nos circuitos integrados, capacitores e indutores por exempo, raramente podem ser colocados, pois o tamanho do componente real é consideravel. Desse modo, os terminais externos do circuito integrado, além de servir para alimentação, entrada e saida de dados, visam a conecção de componentes que não podem ser inseridos dentro do circuito integrado. 

Circuitos integrados existem comercialmente para as mais diversas funções, tais como microprocessadores, memórias, portas logicas, osciladores, circuitos de radio frequencia, entre outros. Um destaque interessante é dado aos circuitos integrados denominados amplificadores operacionais, que são circuitos construidos para amplificar pequenos sinais, com base nas seguintes caracteristicas: 

 - Altissima impedancia de entrada
 - Baixa impedancia de saída
 - Alimentação simétrica
 - Amplificação diferencial das entradas
 - Amplificação com fator de ganho controlado por componentes externos

O amplificador operacional mais popular é o que tem o código 741. Além dele, é bastante usual o LM 324, que consiste de 4 amplificadores em um mesmo encapsulamento, tal como ocorre com circuitos integrados que contem 4 portas logicas E ou OU.

O simbolo elétrico de um amplificador operacional é o seguinte:

![circ-op](https://cloud.githubusercontent.com/assets/3441126/11034017/34458906-86cf-11e5-832e-bbd5881d4453.png)


Esse tipo de circuito é analógico por essencia, e portanto, não se comporta como uma porta digital. Para compreender o seu funcionamento nós devemos lembrar que além da altissima impedancia de entrada de ambas as portas, deve ser levado em conta que ambos os terminais são automaticamente colocados no mesmo potencial eletrico internamente, fato esse conhecido popular mente como terra virtual.
O modelo mais básico para uso desse circuito é o seguinte:

![circ-op-ali-simetrica](https://cloud.githubusercontent.com/assets/3441126/11034019/3563cca8-86cf-11e5-9619-26f4b01d0b23.png)


Funcionamento do Circuito:

> img anotações

![anot](https://cloud.githubusercontent.com/assets/3441126/11034693/a6d2f8fa-86d4-11e5-929d-b1c5ef211961.png)

Com base no equacionamento acima, entendemos que a configuração circuital exibida constitui um amplificador inversor no qual o ganho, ou o fator de amplificação é dado pela divisão de **rb** por **ra**. Notamos que este fator de amplificação pode variar consideravelmente mediante a nossa escolha para os valores dos resistores, entretanto, devemos considerar alguns limites inerentes ao funcionamento do circuito integrado. Primeiramente, entendemos que o uso de **rb** infinito, isto é, inesistente na pratica, não conduz a um ganho infinito, mas sim ao ganho maximo do aplificador, que pode ser de 10 mil ou 100 mil vezes. Da mesma forma, **ra** extremamente pequeno, isto é, tendento a 0 ohm (curto circuito), não conduz a um ganho infinito. De qualquer forma, se considerarmos ambas as situações extremas para **ra** e **rb** teremos o seguinte circuito:

![caso_comparador](https://cloud.githubusercontent.com/assets/3441126/11034512/3aa63472-86d3-11e5-942f-a0f8ee17d266.png)


Este circuito faz com que tenhamos o que se chama de **comparador**, pois quando a entrada **E** for minimamente diferente de 0, o amplificador terá ganho maximo e produzirá na saída **S* a maxima tensão disponível, que é a tensão da fonte.

Por outro lado, uma outra situação extrema é aquela na qual fazemos **rb** tender a 0 e curto-circuitamos uma das entradas à saída, conforme segue:

![curto-circ](https://cloud.githubusercontent.com/assets/3441126/11034575/be85d356-86d3-11e5-95af-0d3e681639fd.png)

Nesse circuito, comunmente chamado de **seguidor de tensao**, **S** é sempre igual a **E**, portanto o ganho é 1. Embora este circuito possa parecer sem uso, pois a saída é sempre identica a entrado, ele é muito utilizado na pratica, pois, sendo a impedancia de entrada altissima, os circuitos de entrada e de saída estão isolados eletricamente. Desse modo, o circuito funciona como um **espelho**.

Temos ainda duas configurações muito comuns envolvendo amplificadores computacionais, que são as seguintes:

 - Amplificador somador

![ampl_somador](https://cloud.githubusercontent.com/assets/3441126/11034759/1f5ea08a-86d5-11e5-9989-8e9aa6579408.png)

 - Amplificador subtrator

![ampl_sub](https://cloud.githubusercontent.com/assets/3441126/11035014/bcabf4cc-86d6-11e5-9e40-f12293b62e12.png)



Inúmeros outros circuitos, não detalhados aqui por estarem fora do escopo deste curso existem, tais como o diferenciador e o integrador que são aqueles nos quais respectivamente **RA** e **Rb** são substituidos por capacitores.

---------------

### MINIPROVA 8
 - Deduzir o equacionamento do circuito subtrator, com base na segunda parte da formulação usada para o circuito amplificador. Após encontrar a corrente no divisor de tensão formado por RA e RB ligado na porta inversora, observar que, para concluir o equacionamento, a tensão em RB não é **S-0 = S**, mas sim a subtração de S pela tensão fornecida pelo divisor de tensão da porta não inversora.


### Projeto Prático

Construíremos um circuito transmissor de radio-frequência com portadora em 96 Mhz e modulação em frequência (FM). Na entrada, injetaremos um sinal acustico oriundo da placa de áudio do computador ou de outro emissor acústico qualquer. O sinal deve ser recebido em qualquer receptor de FM comum nas proximidades do circuito. Passaremos a definição do cirucito eletrônico e a correspondente confecção da placa de circuito impresso em fibra de vidro utilizando decalque eletrônico. 
