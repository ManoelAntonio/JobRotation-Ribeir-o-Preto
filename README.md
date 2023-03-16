# JobRotation-Ribeirao-Preto
Teste tecnico-Target Sistemas

PERGUNTAS
1) Observe o trecho de código abaixo:

int INDICE = 13, SOMA = 0, K = 0;

enquanto K < INDICE faça

{

K = K + 1;

SOMA = SOMA + K;

}

imprimir(SOMA);



Ao final do processamento, qual será o valor da variável SOMA?



2) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.



IMPORTANTE:

Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;



3) Descubra a lógica e complete o próximo elemento:



a) 1, 3, 5, 7, ___

b) 2, 4, 8, 16, 32, 64, ____

c) 0, 1, 4, 9, 16, 25, 36, ____

d) 4, 16, 36, 64, ____

e) 1, 1, 2, 3, 5, 8, ____

f) 2,10, 12, 16, 17, 18, 19, ____



4 - Dois veículos (um carro e um caminhão) saem respectivamente de cidades opostas pela mesma rodovia. O carro de Ribeirão Preto em direção a Franca, a uma velocidade constante de 110 km/h e o caminhão de Franca em direção a Ribeirão Preto a uma velocidade constante de 80 km/h. Quando eles se cruzarem na rodovia, qual estará mais próximo a cidade de Ribeirão Preto?



IMPORTANTE:

a) Considerar a distância de 100km entre a cidade de Ribeirão Preto <-> Franca.

b) Considerar 2 pedágios como obstáculo e que o caminhão leva 5 minutos a mais para passar em cada um deles e o carro possui tag de pedágio (Sem Parar)

c) Explique como chegou no resultado.

 

5) Escreva um programa que inverta os caracteres de um string.


RESPOSTAS

01) Acredito que o resultado final da variável SOMA será 91. Isso porque o loop é executado 13 vezes, somando os valores de K em cada iteração. Como o valor inicial de K é 1 e o valor final é 13, a soma total será de 1+2+3+...+13, que é igual a 91.

2) 
let num = prompt("Digite um número:");

let a = 0;
let b = 1;
let c;

while (b <= num) {
  if (num == b) {
    alert(num + " pertence à sequência de Fibonacci.");
    break;
  }
  c = a + b;
  a = b;
  b = c;
}

if (num != b) {
  alert(num + " não pertence à sequência de Fibonacci.");
}

03)
a)9
b)128
c)49
d)100
e)13
f)20

04) Quando os veículos se cruzarem na rodovia, o caminhão estará mais próximo da cidade de Ribeirão Preto. Isso ocorre porque o caminhão leva mais tempo para percorrer a mesma distância que o carro, devido aos pedágios. Mesmo com uma velocidade menor, o caminhão percorre um trecho menor da estrada e, portanto, chega mais perto de Ribeirão Preto do que o carro.


05)
let stringOriginal = "Exemplo de string a ser invertida";
let stringInvertida = "";

for(let i = stringOriginal.length - 1; i >= 0; i--){
    stringInvertida += stringOriginal[i];
}

console.log("String original: " + stringOriginal);
console.log("String invertida: " + stringInvertida);







