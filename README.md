# 🔎 Pesquisador de Fibonacci (Escala Infinita)

Este projeto é uma aplicação web simples que permite consultar termos da sequência de Fibonacci, incluindo índices extremamente grandes, utilizando uma **aproximação matemática baseada em logaritmos e Fórmula de Binet**.

A interface aceita números sem limite prático e retorna o valor estimado do termo em **notação científica**, preservando desempenho mesmo para entradas gigantescas.

---

## 🚀 Demonstração

Digite qualquer número inteiro positivo e obtenha o termo correspondente da sequência de Fibonacci.
Para números pequenos, o valor é exato. Para números muito grandes, o resultado é uma **aproximação altamente precisa da ordem de grandeza**.

---

## 🧠 Como funciona

O projeto utiliza uma versão otimizada da **Fórmula de Binet**, combinada com logaritmos base 10 para evitar estouro de memória e cálculos pesados:

* Usa constantes pré-calculadas:

  * `log10(φ)` onde φ é o número áureo
  * `log10(√5)`
* Transforma o cálculo em uma operação de escala logarítmica
* Separa o resultado em:

  * **mantissa** (parte significativa do número)
  * **expoente** (quantidade de dígitos em base 10)

Isso permite estimar termos extremamente grandes da sequência sem calcular os valores reais.

---

## ✨ Funcionalidades

* 📌 Cálculo de Fibonacci para números pequenos (exato)
* 📌 Suporte a índices extremamente grandes (aproximado)
* 📌 Saída em notação científica legível
* 📌 Exibição da quantidade total de dígitos do termo
* 📌 Interface responsiva e simples
* 📌 Processamento rápido com debounce (evita travamentos)

---

## 📦 Estrutura

O projeto é composto por um único arquivo HTML contendo:

* Estrutura da interface
* Estilos básicos inline
* Lógica JavaScript para cálculo da sequência

---

## ▶️ Como usar

1. Baixe ou copie o arquivo `.html`
2. Abra em qualquer navegador moderno
3. Digite um número no campo de entrada
4. Veja o resultado automaticamente

---

## ⚠️ Observações

* Para valores pequenos (0 a 9), os resultados são exatos.
* Para valores muito grandes, o resultado é uma **aproximação matemática da magnitude do termo**, não o número completo (que seria impraticável de calcular).

---

## 📚 Base matemática

* Sequência de Fibonacci
* Fórmula de Binet
* Logaritmos e notação científica
* Propriedades do número áureo (φ)

---

## 🛠️ Possíveis melhorias

* Separar JS em arquivo externo
* Adicionar gráficos de crescimento da sequência
* Criar versão com Web Worker para cálculos paralelos
* Suporte a precisão arbitrária (BigInt + bibliotecas matemáticas)
