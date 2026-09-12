# 🌿 Kaa Examples of Codes

Este repositório é dedicado a exemplos práticos de implementação utilizando a linguagem **Kaa**, um projeto de linguagem de programação que combina clareza didática, segurança de tipos e alta performance via execução em C.

## 📖 Sobre a Linguagem Kaa

A **Kaa** (nome derivado de *Nheengatu* para "Folha/Floresta") é uma linguagem que pertence às famílias de sintaxe e design do **C** e do **Python**. Ela foi projetada sob uma filosofia orgânica, onde a memória e os escopos funcionam como um ecossistema: surgem para cumprir seu papel e são descartados eficientemente para nutrir novas execuções.

### 🚀 Pilares Técnicos
- **C-Bound JIT & Cython VM:** A Kaa não é apenas interpretada; ela compila código para bytecode denso executado por uma Máquina Virtual implementada em Cython, permitindo performance próxima ao C nativo.
- **Tipagem Explícita por Flags:** Diferente de linguagens dinâmicas, a Kaa utiliza flags obrigatórias para declaração de variáveis, eliminando ambiguidades e otimizando a VM.
  - `-i` (Inteiro), `-f` (Float), `-s` (String), `-T/-F` (Booleanos), `-l` (Lista), `-t` (Tupla), `-d` (Dicionário), `-obj` (S-Bot).
- **Strict Scope (Regra de Ouro):** Isolamento absoluto de funções. É proibido ler ou alterar variáveis globais de dentro de funções sem passá-las explicitamente como parâmetros, eliminando bugs de estado global.
- **S-Bots (Orientação a Objetos):** Implementa POO via *Factory Patterns* e *Closures*. Objetos (S-Bots) são entidades dinâmicas com estado encapsulado e despacho de métodos otimizado.
- **Gerenciamento por Arenas:** A memória é organizada em Arenas isoladas, permitindo que módulos inteiros sejam deletados da memória em tempo constante $O(1)$ via `destroy_arena()`.

### 🛠️ Recursos Avançados
- **Operadores Atômicos:** Possui operadores como `!or` (NOR), `xor` (OU Exclusivo), `in` e `!in` para verificações rápidas de pertinência.
- **Interpolação de Strings:** Suporte a strings dinâmicas com a sintaxe `$"Texto {variavel}"` e suporte a strings triplas `\"\"\"` para blocos multilinha.
- **Interoperabilidade Python:** Integração nativa com o ecossistema CPython através da flag `add -py`, permitindo usar bibliotecas como `numpy` ou `math` do Python diretamente no código Kaa.
- **Coerção Segura:** Proteção contra truncamento silencioso de números (ex: tentar atribuir `10.5` a um `-i` gera erro imediato em vez de arredondar).

## 📂 O que você encontrará aqui
Neste repositório, você verá exemplos de:
- Algoritmos implementados em Kaa.
- Estruturas de S-Bots para simulações e sistemas.
- Uso de Arenas para gerenciamento de memória.
- Integrações híbridas Kaa $\leftrightarrow$ Python.


