# progamas-de-fixa-ao-tipos-primitivos 
// 1. Pegar o nome e a idade e exibir
let nome = 'Muriel Bezerra';
let idade = '19';
console.log(`Seu nome é '${nome}' e você tem ${idade} anos.`);

// 2. Pegar o nome e a cidade
let cidade = prompt('Digite a cidade onde você mora:');
console.log(`${nome} mora em ${cidade}.`);

// 3. Operações matemáticas
let numero1 = parseInt(prompt('Digite o primeiro número: '));
let numero2 = parseInt(prompt('Digite o segundo número: '));
const soma = numero1 + numero2;
const subtracao = numero1 - numero2;
const multiplicacao = (numero1 * numero2).toFixed(2);
const divisao = (numero1 / numero2).toFixed(2);
console.log(`A soma é ${soma}`);
console.log(`A subtração é ${subtracao}`);
console.log(`A multiplicação é ${multiplicacao}`);
console.log(`A divisão é ${divisao}`);

// 4. Calcular área do triângulo
let base = parseInt(prompt(`Digite a base do triângulo: `));
let altura = parseInt(prompt(`Digite a altura do triângulo: `));
const area = ((base * altura) / 2).toFixed(2);
console.log(`A base do triângulo é: ${base}`);
console.log(`A altura do triângulo é: ${altura}`);
console.log(`A área do triângulo é: ${area}`);

// 5. Calcular a média de 3 notas
let nota1 = parseInt(prompt(`Digite a primeira nota: `));
let nota2 = parseInt(prompt(`Digite a segunda nota: `));
let nota3 = parseInt(prompt(`Digite a terceira nota: `));
const media = ((nota1 + nota2 + nota3) / 3).toFixed(2);
console.log(`A média das notas é: ${media}`);

// 6. Produto com desconto
let produto = parseFloat(prompt('Digite o valor do produto:'));
const desconto = 0.5; // 50% de desconto
let valorDesconto = produto * desconto;
let valorFinal = produto - valorDesconto;
console.log(`O valor do produto é ${produto.toFixed(2)}. Com o desconto de 50%, o valor final é ${valorFinal.toFixed(2)}.`);

// 7 Imposto de Renda 
let salarioBruto = parseFloat(prompt("Digite seu salário bruto:"));
let aliquota;

if (salarioBruto <= 1903.98) {
  aliquota = 0;
} else if (salarioBruto <= 2826.65) {
  aliquota = 0.075; // 7,5%
} else if (salarioBruto <= 3751.05) {
  aliquota = 0.15; // 15%
} else if (salarioBruto <= 4664.68) {
  aliquota = 0.225; // 22,5%
} else {
  aliquota = 0.275; // 27,5%
}

let imposto = (salarioBruto * aliquota).toFixed(2);

let salarioLiquido = (salarioBruto - imposto).toFixed(2);

console.log(`Seu salário bruto é R$${salarioBruto.toFixed(2)}.`);
console.log(`O imposto de renda a ser pago é ${imposto}.`);
console.log(`Seu salário líquido após o imposto é ${salarioLiquido}.`);


//8 Conversor de Moedas
let valorEmReal = parseFloat(prompt("Digite o valor em Reais (BRL):"));
const taxaCambio = 0.19; 
let valorEmDolar = (valorEmReal * taxaCambio).toFixed(2);

console.log(`O valor de R$${valorEmReal.toFixed(2)} convertido para dólares (USD) é ${valorEmDolar}.`);
 // 9 Conversão de Celsius para Fahrenheit
let tempCelsius = parseFloat(prompt("Digite a temperatura em Celsius:"));
let tempFahrenheit = ((tempCelsius * 9/5) + 32).toFixed(2);

console.log(`A temperatura de ${tempCelsius}°C corresponde a ${tempFahrenheit}°F.`);
 
//10 Calculadora de IMC
let peso = parseFloat(prompt("Digite seu peso (em kg):"));
let altura = parseFloat(prompt("Digite sua altura (em metros):"));

let imc = (peso / (altura * altura)).toFixed(2);

console.log(`Seu IMC é ${imc}.`);

