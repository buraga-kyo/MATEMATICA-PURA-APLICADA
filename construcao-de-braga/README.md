# Construção de Braga

eu imaginei o infinito e refleti...  

o universo é um espelho circular causando EFEITO de infinito...  

logo falei EUREKA o infinito é apenas um efeito, coloque um espelho na frente do outro, existe um efeito de infinito, no universo, porem, mais denso e profundo a ponto de causar quase uma alucinação sinergica; é como se a gente fosse esse * e o universo ( ) nos estamos no meio ( * ) imagine que o ( ) é um circulo ok e nos estamos no meio, pra qualquer lugar que a gente olhar reflete meio que tudo, imagine um espelho circular gigante e voce no meio dele ou melhor, no inicio dele... agora olhe pra qualquer lugar, advinha oque acontece se fosse apenas ampliar a camera ??? isso mesmo é inifinito para sempre, mas é so um efeito.... enfim pensei como eu posso representar isso com numero?  

ja sei !!  

010203040506070809  
908070605040302010  
  
 1 2 3 4 5 6 7 8 9  
9 8 7 6 5 4 3 2 1  
  
918273645546372819  
  
EUREKA  
  
desde então venho procurando padrões nesse numero 918273645546372819 (dias despois descobri que foi uma re-descorbeta kkk isso existe e é a sequência A078271)

voce entendeu como cheguei nele? eu liguei a sequencia numero com zero, para não termos o problem do infinito entre 1, 2, 3... depois refleti ele como o universo, ai pensei ok, e se eu tirar os zeros e descer a coluna de cima para baixo?.... para não ter que ficar escrevendo tantos numeros é tipo as duas colunas iniciais zipadas. enfim me deparei com esse numero que é tipo:  

oi meu nome é espelho, eu tenho propriedades que gritam ESPELHO ESPELHO ESPEEEEEEEEEEEELHO;

oque isso quer dizer né? kkk é tipo assim vamos partir do principio que

escolha qualquer numero que da pra contar com os dedos... 7 por exemplo  

vamos construir sua sequencia com zeros  
01020304050607  

agora vamos refletir ele como num espelho circular  
70605040302010  

agora vamos por um embaixo do outro  
01020304050607  
70605040302010  

agora vamos tirar os zeros  
 1 2 3 4 5 6 7  
7 6 5 4 3 2 1  

agora vamos descer a primeira coluna para termos uma sequencia de uma linha  
e pronto temos que ℬ(7) = 71625344352617  

para não ter que falar 1 kilo de texto sempre e explicar o caminho do pensar toda hora podemos resumir toda essa logica em:  

$$
\text{ℬ}(n) = \bigoplus_{i=1}^{n} \left( (n - i + 1), i \right)
$$

isso vale para qualquer numero sem virgula maior que 1 (eu to tentando ao maximo não usar nenhum jargão matematico kkk e é aqui onde a sequência A078271 deixa de fazer sentido, quando se entra com um numero maior que 10, ainda não fiz uma bateria de testes mas deixam de ser palindromos)

02/set/1898 - 20:77
Bom comecei a fazer uma bateria de testes e acabei descobrindo algo interessante de uma fonte simples; Se a gente olhar para a sequencia 918273645546372819 e separar por blocos, exemplo: 9182 vamos ver que a tabuada do 9 de 2 ao 9 o resultado sempre esta a frente do multiplicador, em 9182 9x2=18, em 273 9x3=27, em 455 9x5=45... então a sequencia tem essa propriedade que ainda não sei o nome, mas explicando sem nome técnico é; pegue a tabuada do nove de 2x9 ate 9x9 e escreva ela em uma linha com o 9 na frente iniciando a sequencia, então, temos: 9 18 27 36 45... ai a gente junta tudo tlg 918273645546372819; E foi pensando nisso que eu falei qual seria fabrica de numeros que imprime a tabuada em uma linha? com toda minha capacidade de pesquisa eu não consegui encontrar uma pronta na presenta data que vai ser lavrada nesse commit, então resolvi criar a fabrica; ela basicamente faz isso que eu falei com qualquer numero maior que 2 que você entrar, e calma, tem algo bizarramente interessante depois que comecei a construir percebi alguns padrões, enfim EU O Geômetra desta casa apresento a Fabrica de tabuada:  

$$
\text{ℱ}_{\infty}(t) = t \oplus \bigoplus_{m=2}^{\infty} \left( (t \cdot m) \oplus m \right)
$$  

bom o ℱ todo bonitão escrito com aquela caneta de pena é de Fabrica e o simbolo do infito depois é de "não para de fazer essa porra nunca mais" o t é o numero que você quer que vire a sequencia da tabuada tipo ℱ(9) vai imprimir 918273645546372819... e logo apos eu tenho o t que é para começar com o numero escolhido, se não a sequencia começaria assim: 18273645546372819.... sem o 9. o camaradinha aqui ⊕ é para criar de fato uma sequencia sem soma ou seja um resultado na frente do outro; o ⊕ grandão com m=2 em baixo e infinito em cima está falando assim: começa a partir do 2 e vai ate o infinito e além... (t·m) é literalmente a tabuada né 9x2, 9x3... depois vc cola o multiplicador do lado do resultado da tabuada é o m e depois segue pro proximo multiplicador da tabuada. é basicamente isso que essa formula esta falando, mas eu preciso encontrar algo melhor que o ⊕ para isso porque com o ⊕ eu preciso explicar pra outro matematico que é CONCATENAÇÃO CONCATENAÇÃO... eu quero um que ja fale isso, porq esse cara pode ser usado pra outras coisas mas enfim bora pros resultados:  

vamos mudar rapidamente o infinito da fabrica para de m=2 a 9, para facilitar a primeira leitura:
  
ℱ(2) = 2426384105126147168189  
ℱ(3) = 36293124155186217248279  
ℱ(4) = 482123164205246287328369  
ℱ(5) = 5102153204255306357408459  
ℱ(6) = 6122183244305366427488549  
ℱ(7) = 7142213284355426497568639  
ℱ(8) = 8162243324405486567648729  
ℱ(9) = 9182273364455546637728819  

tem alguns padrões interessantes, o penultimo numero é decescente e o antipenultimo é crescente, mas de longe o mais interessante é; Vamos voltar a fabrica original até o inifito, para qualquer numero que você entrar ℱ(9) por exemplo, é uma sequencia DISJUNTIVA, isso quer dizer que seu CPF, seu numero de celular, sua senha e seu numero de cartão de credito aparece nessa sequencia ;) QUALQUER SENHA, CPF, NUMERO DA MEGA SENA do mundo aparece nesse caralho aqui, vlw vou dormir.

Obs1: eu sei quem é David Gawen Champernowne

Bom em uma era de IA esta cada vez mais importante ser humano! estudar as pessoas do passado é o proximo passo para evolução! [musica de fundo dramatica]

Ah uma dica em vez de usar IA para entender oque está sendo desvendado e/ou inventado agora; procure pensar por conta propria, IA não pensa mas você pode, experimente ;)
