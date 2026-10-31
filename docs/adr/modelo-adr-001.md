# ADR-001 — Preparar o repositório da equipe

- **Situação:** aceita
- **Data:** 2026-10-31
- **Participantes:** Joao Vitor, Andrey Vinicius, Gabriel Florenco, Mateus Borges

## Contexto

Foi decidido durante a aula que o sistema utilizará a arquitetura MVC (Model-View-Controller) organizada como um monólito modular.

A equipe é composta por quatro integrantes e precisa trabalhar no mesmo repositório de forma organizada, permitindo que diferentes partes do sistema sejam desenvolvidas separadamente sem transformar o projeto em vários sistemas independentes.

A utilização de um monólito modular permite manter uma única aplicação e um único repositório, facilitando a execução e a implantação do sistema, enquanto a divisão em módulos ajuda a separar responsabilidades e reduzir o acoplamento entre as funcionalidades.

## Decisão

O projeto será desenvolvido utilizando a arquitetura MVC aplicada em um monólito modular.

O sistema será dividido em módulos de acordo com as funcionalidades ou domínios definidos pela equipe, mantendo uma estrutura organizada dentro de uma única aplicação e seguindo a separação de responsabilidades entre Model, View e Controller.

## Alternativas consideradas

Alternativa                 | Por que não foi escolhida
MVC sem modularização       | Poderia dificultar a organização do projeto conforme o sistema crescesse, concentrando muitas funcionalidades na mesma estrutura.
Microserviços               | Adicionaria complexidade desnecessária para o tamanho atual do projeto e da equipe, exigindo comunicação entre serviços, implantação separada e maior infraestrutura.
Monólito tradicional        | Possui uma estrutura mais simples inicialmente, mas pode se tornar desorganizado e mais difícil de manter caso todas as funcionalidades fiquem muito acopladas.
Clean Architecture completa | Poderia adicionar uma complexidade maior do que a necessária para o projeto e aumentar o tempo de desenvolvimento e aprendizado da equipe.

## Consequências

- **Positivas:** A equipe poderá trabalhar em módulos diferentes dentro do mesmo projeto, mantendo uma única aplicação e uma estrutura mais organizada. A separação entre Model, View e Controller também facilita a manutenção e a divisão das responsabilidades.
- **Negativas:** Será necessário manter disciplina na organização dos módulos para evitar dependências indevidas entre eles. A equipe também precisará definir claramente os limites e responsabilidades de cada módulo.
- **Como verificar:** urante as revisões de código, será verificado se as novas funcionalidades estão sendo adicionadas ao módulo correto e se a separação entre Model, View e Controller está sendo respeitada. Também será analisado se os módulos evitam dependências diretas desnecessárias entre si.
