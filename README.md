# Lista de Exercícios em Kotlin

---

## Exercício 01 – Conversão de Celsius para Fahrenheit

**Enunciado:** Converter Celsius para Fahrenheit.

```kotlin
fun main() {
    println("Insira o valor em Celsius:")
    val celsius = readln().toDouble()

    val fahrenheit = (1.8 * celsius) + 32
    println("Seu valor em Fahrenheit é: $fahrenheit")
}
```

---

## Exercício 02 – Conversão de Fahrenheit para Celsius

**Enunciado:** Converter Fahrenheit para Celsius.

```kotlin
fun main() {
    println("Insira o valor em Fahrenheit:")
    val fah = readln().toDouble()

    val celsius = (fah - 32) * 5.0 / 9.0
    println("Seu valor em Celsius é: $celsius")
}
```

---

## Exercício 03 – Volume de uma Lata de Óleo

**Enunciado:** Volume de uma lata de óleo.

```kotlin
fun main() {
    println("Insira o valor do raio da base em centímetros:")
    val raio = readln().toDouble()

    println("Insira o valor da altura em centímetros:")
    val altura = readln().toDouble()

    val volume = Math.PI * raio * raio * altura
    println("O volume é: $volume")
}
```

---

## Exercício 04 – Combustível Gasto em uma Viagem

**Enunciado:** Quantidade de litros de combustível gasta em uma viagem.

```kotlin
fun main() {
    print("Insira a distância: ")
    val distancia = readln().toDouble()

    print("Insira o consumo (km por litro): ")
    val consumo = readln().toDouble()

    val litros = distancia / consumo
    println("Combustível gasto: $litros litros")
}
```

---

## Exercício 05 – Prestação em Atraso

**Enunciado:** Valor de uma prestação em atraso.

```kotlin
fun main() {
    println("Insira o valor original:")
    val valorOriginal = readln().toDouble()

    println("Insira a quantidade de meses:")
    val meses = readln().toInt()

    println("Insira a taxa:")
    val taxa = readln().toDouble()

    val valor = valorOriginal + (valorOriginal * (taxa / 100) * meses)
    println("Valor a pagar: R$$valor")
}
```

---

## Exercício 06 – Troca de Valores

**Enunciado:** Troca de valores entre duas variáveis.

```kotlin
fun main() {
    print("Digite o valor de A: ")
    var a = readln()

    print("Digite o valor de B: ")
    var b = readln()

    val aux = a
    a = b
    b = aux

    println("A = $a")
    println("B = $b")
}
```

---

## Exercício 07 – Soma e Multiplicação de Quatro Números

**Enunciado:** Adição e multiplicação de quatro números inteiros.

```kotlin
fun main() {
    val lista = mutableListOf<Int>()

    repeat(4) {
        lista.add(readln().toInt())
    }

    val soma = lista.sum()
    val multiplicacao = lista.reduce { acc, i -> acc * i }

    println("Soma: $soma")
    println("Multiplicação: $multiplicacao")
}
```

---

## Exercício 08 – Volume de uma Caixa Retangular

**Enunciado:** Valor do volume de uma caixa retangular.

```kotlin
fun main() {
    val comprimento = readln().toDouble()
    val largura = readln().toDouble()
    val altura = readln().toDouble()

    val volume = comprimento * largura * altura
    println("Volume: $volume")
}
```

---

## Exercício 09 – Número ao Quadrado

**Enunciado:** Número inteiro ao quadrado.

```kotlin
import kotlin.math.pow

fun main() {
    val numero = readln().toDouble()
    val resultado = numero.pow(2.0)
    println("Resultado: $resultado")
}
```

---

## Exercício 10 – Diferença entre Dois Números

**Enunciado:** Diferença do primeiro número pelo segundo.

```kotlin
fun main() {
    val a = readln().toDouble()
    val b = readln().toDouble()

    val resultado = a - b
    println("Diferença: $resultado")
}
```

---

## Exercício 11 – Conversão de Dólar para Real

**Enunciado:** Conversão do dólar para o real.

```kotlin
fun main() {
    val valor = readln().toDouble()
    val calculo = valor * 5.60
    println("Valor em real: R$$calculo")
}
```

---

## Exercício 12 – Conversão de Real para Dólar

**Enunciado:** Conversão do real para o dólar.

```kotlin
fun main() {
    val valor = readln().toDouble()
    val calculo = valor / 5.60
    println("Valor em dólar: $calculo")
}
```

---

## Exercício 13 – Soma dos Quadrados de Três Números

**Enunciado:** Soma dos quadrados de três números.

```kotlin
fun main() {
    val n1 = readln().toInt()
    val n2 = readln().toInt()
    val n3 = readln().toInt()

    val soma = (n1 * n1) + (n2 * n2) + (n3 * n3)
    println("Resultado: $soma")
}
```

---

## Exercício 14 – Quadrado da Soma de Três Números

**Enunciado:** Cálculo do quadrado da soma de três números.

```kotlin
import kotlin.math.pow

fun main() {
    val a = readln().toDouble()
    val b = readln().toDouble()
    val c = readln().toDouble()

    val resultado = (a + b + c).pow(2)
    println("Resultado: $resultado")
}
```

---

## Exercício 15 – Produto e Soma de Quatro Números

**Enunciado:** Cálculo do produto e da soma de quatro números.

```kotlin
fun main() {
    val lista = mutableListOf<Int>()

    repeat(4) {
        lista.add(readln().toInt())
    }

    val produto = lista[0] * lista[2]
    val soma = lista[1] + lista[3]

    println("Soma: $soma")
    println("Produto: $produto")
}
```

---

## Exercício 16 – Novo Salário com Aumento

**Enunciado:** Cálculo do novo salário com aumento.

```kotlin
fun main() {
    val salario = readln().toDouble()
    val porcentagem = readln().toDouble()

    val aumento = salario * (porcentagem / 100)
    val novoSalario = salario + aumento

    println("Novo salário: $novoSalario")
    println("Aumento: $aumento")
}
```

---

## Exercício 17 – Área de uma Circunferência

**Enunciado:** Cálculo da área de uma circunferência.

```kotlin
fun main() {
    val raio = readln().toDouble()
    val area = Math.PI * raio * raio
    println("Área: $area")
}
```

---

## Exercício 18 – Apuração de Votos

**Enunciado:** Apuração de votos em uma eleição sindical.

```kotlin
fun main() {
    val a = readln().toDouble()
    val b = readln().toDouble()
    val c = readln().toDouble()
    val d = readln().toDouble()
    val e = readln().toDouble()

    val total = a + b + c + d + e

    println((a / total) * 100)
    println((b / total) * 100)
    println((c / total) * 100)
    println((d / total) * 100)
    println((e / total) * 100)
}
```

## Exercício 19 – Cálculo das Quatro Operações Básicas

**Enunciado:** Ler dois números e calcular soma, subtração, multiplicação e divisão.

```kotlin
fun main() {
    val lista = mutableListOf<Int>()

    repeat(2) {
        lista.add(readln().toInt())
    }

    val soma = lista[0] + lista[1]
    val subtracao = lista[0] - lista[1]
    val produto = lista[0] * lista[1]
    val quociente = lista[0] / lista[1]

    println("Soma: $soma")
    println("Subtração: $subtracao")
    println("Produto: $produto")
    println("Quociente: $quociente")
}
```

---

## Exercício 20 – Cálculo da Velocidade de um Projétil

**Enunciado:** Calcular a velocidade média em m/s.

```kotlin
fun main() {
    val km = readln().toDouble()
    val horas = readln().toDouble()

    val ms = (km * 1000) / (horas * 3600)
    println("Velocidade: $ms m/s")
}
```

---

## Exercício 21 – Cálculo de Potência

**Enunciado:** Calcular a potência de um número.

```kotlin
fun main() {
    val base = readln().toDouble()
    val expoente = readln().toDouble()

    val resultado = Math.pow(base, expoente)
    println("Resultado: $resultado")
}
```

---

## Exercício 22 – Volume de uma Esfera

**Enunciado:** Calcular o volume de uma esfera.

```kotlin
fun main() {
    val raio = readln().toDouble()

    val volume = (4.0 / 3.0) * Math.PI * (raio * raio * raio)
    println("Volume: $volume")
}
```

---

## Exercício 23 – Conversão de Metros para Pés

**Enunciado:** Converter metros para pés.

```kotlin
fun main() {
    val metros = readln().toDouble()

    val pes = metros / 0.3048
    println("Valor em pés: $pes")
}
```

---

## Exercício 24 – Cálculo de Raiz

**Enunciado:** Calcular a raiz de um número.

```kotlin
fun main() {
    val base = readln().toDouble()
    val indice = readln().toDouble()

    val raiz = Math.pow(base, 1.0 / indice)
    println("Resultado: $raiz")
}
```

---

## Exercício 25 – Sucessor e Antecessor

**Enunciado:** Calcular o sucessor e o antecessor de um número inteiro.

```kotlin
fun main() {
    val numero = readln().toInt()

    val sucessor = numero + 1
    val antecessor = numero - 1

    println("Sucessor: $sucessor")
    println("Antecessor: $antecessor")
}
```

---

## Exercício 26 – Quadrado da Divisão de Dois Números

**Enunciado:** Calcular o quadrado do resultado da divisão de dois números.

```kotlin
fun main() {
    val a = readln().toDouble()
    val b = readln().toDouble()

    val divisao = a / b
    val quadrado = divisao * divisao

    println("Resultado da divisão: $divisao")
    println("Quadrado do resultado: $quadrado")
}
```

---
