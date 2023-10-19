---
theme: "night"
transition: "slide"
title: "C4 - Model"
enableMenu: false
enableSearch: false
enableChalkboard: false
---

### Documentação de projetos

![-](./images/doc.svg){ width=70% }

---

### O que veremos hoje


---

### O que veremos hoje

- Documentação

---

### O que veremos hoje

- Documentação
- Readme

---

### O que veremos hoje

- Documentação
- Readme
- C4 Model

---

### O que veremos hoje

- Documentação
- Readme
- C4 Model
- Diagram As Code

---

## Documentar?

---

#### Software em funcionamento mais que documentação abrangente - Manifesto Ágil

---

#### Alguns "traduzem" essa frase como: 
#### NÃO documentar nada!

---

### Na maioria dos casos precisamos documentar, nem que seja o básico!

---

## Por quê documentar?


---

#### Por quê documentar?

- Onboarding de pessaos no time

---

#### Por quê documentar?

- Onboarding de pessaos no time
- Não ficar dependendo de só uma pessoa

---

#### Por quê documentar?

- Onboarding de pessaos no time
- Não ficar dependendo de só uma pessoa
- Facilidade na comunicação / discussões

---

#### Por quê documentar?

- Onboarding de pessaos no time
- Não ficar dependendo de só uma pessoa
- Facilidade na comunicação / discussões
- Teu código fonte não conta toda história


---

#### Por quê documentar?

- Onboarding de pessaos no time
- Não ficar dependendo de só uma pessoa
- Facilidade na comunicação / discussões
- Teu código fonte não conta toda história
- ...

---

#### Mas esta sempre desatualizado...

---

#### Mesmo assim, teremos uma ideia de onde estamos! E não vai ser tudo que vai estar desatualizado.


---

## Por onde começar?

---

### Readme

![-](./images/readme.svg)

---

## O que colocar?


---

### O que colocar?

- Qual o objetivo do projeto

---

### O que colocar?

- Qual o objetivo do projeto
- O que precisa ser instalado

---

### O que colocar?

- Qual o objetivo do projeto
- O que precisa ser instalado
- Como rodar o projeto

---

### O que colocar?

- Qual o objetivo do projeto
- O que precisa ser instalado
- Como rodar o projeto
- Dicionário de termos

---

### O que colocar?

- Qual o objetivo do projeto
- O que precisa ser instalado
- Como rodar o projeto
- Dicionário de termos
- Configurações, Migrations, Deploy...

---

### Exemplo

![Fluxo De Caixa](./images/readme-exemplo.png)

[Fluxo De Caixa](https://github.com/CristianoRC/Fluxo-De-Caixa)

---


### Geradores

- https://readme-gen.vercel.app/app

- https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/

- https://readme.so/editor

---

### Dúvidas?

![alt](https://media3.giphy.com/media/3o6MbudLhIoFwrkTQY/giphy.gif?cid=790b76117789c6161150915091725a365bdeac4e06fd01cd&rid=giphy.gif&ct=g){ width=90% }

---

### E a documentação da arquitetura?

---

### Problema


---

### Padronização!


![-](./images/diagram.svg){ width=60% }

---

### Fluxo, Arquitetura, Cloud...

---

![-](./images/nazare.png){ width=80% }

---

#### Mesma solução diferentes desenhos

![-](./images/mind-map.svg){ width=60% }


---

![-](./images/diagramas.png){ width=90% }


---

### UML?
![-](https://cdn-icons-png.flaticon.com/512/5108/5108789.png){ width=30% }

---

### Complexidade
Principalmente na criação, são muitas regras!

---

## 🚀 C4 - Model 📐

![-](./images/Capa.png){ width=55% }

---

### Camadas - 4

![-](https://infostart.ru/upload/iblock/50d/50dd77ec284cca1070600cf82822c5ca.png)


---

**Primeiro, visão geral; depois, amplie e filtre; em seguida, detalhes sob demanda - Ben Shneiderma, 1996**

---

[The Eyes Have It: A Task by Data Type Taxonomy for Information Visualizations](https://www.cs.umd.edu/~ben/papers/Shneiderman1996eyes.pdf)

---

![camadas](./images/camadas.png)

---

### Vai dando zoom nas camadas

![zoom](./images/zoom.svg){ width=50% }

---

![zoom](./images/zoom-1.png)

---

![zoom](./images/zoom-2.png)

---

![zoom](./images/zoom-3.png)

---

![zoom](./images/zoom-4.png)

---

![zoom](./images/zoom-5.png)

---

![zoom](./images/zoom-6.png)

---

![zoom](./images/zoom-7.png)

---

### System Context

Tem como objetivo ser o ponto de entrada, uma visão geral!

---

### System Context - Público alvo

**Pessoas ténicas e não tecnicas**

---

#### System Context - Person

![People](./images/people.png){ width=40% }

---

#### System Context - Software systems

![Sistema](./images/sistema.png){ width=90% }

---

#### System Context - Enterprise boundary

![Sistema](./images/bonduary.png){ width=70% }

<small>Opcional</small>

---

#### System Context - Interações

![Relacionamento](./images/relacionamento.png)

---

#### System Context

![context](./images/context-exemplo.png)

---

## Container

Ter uma visão mais detalhada da arquitetura, quais os serviços fazem parte, e como se comunicam

---

### Container - Público alvo

**Pessoas técnicas, dev, dba, qa...**

---

#### Container - Person

![People](./images/people.png){ width=40% }

---

#### Container - Sistema existente

![Existente](./images/sistema-existente.png){ width=60% }


---

#### Container - Boundary

![Sistema](./images/bonduary.png){ width=70% }

<small>Opcional</small>


---

#### Container

![container](./images/container.png){ width=60% }

---

#### Container - "Clientes"

![app](./images/apps.png){ width=90% }


---

#### Container - Banco de dados

![banco](./images/banco.png){ width=40% }

---

#### Container - Filas / Tópicos

![banco](./images/fila.png){ width=40% }

<small>Há controvérsias</small>

---

#### Container

![container](./images/container-exemplo.png){ width=85% }

---

## Component


---

### Component - Público alvo

**Time que vai desenvolver a solução**

---

#### Component

![-](./images/componente.png){ width=50% }

<small>O unico diferente</small>

---

#### Component

![componente](./images/componente-exemplo.png)

---


## Code

![-](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/UML_logo.svg/800px-UML_logo.svg.png){ width=60% }

---

## Code

![Diagrama de classe](https://www.researchgate.net/publication/225686440/figure/fig3/AS:667828239732738@1536234068086/A-simple-class-diagram-for-a-commercial-software-application-in-UML-notation-The.png){ width=75% }    

---

### Ferramentas

![-](./images/tools.svg){ width=70% }

---

### Miro

![-](./images/Miro.png){ width=85% }

---

### Excalidraw

![-](./images/Excalidraw.png)

---

### Como manter atualizado?

![-](./images/question.svg){ width=60% }

---

### Diagram As Code

![-](./images/programming.svg){ width=60% }

---

## Plant UML

![-](https://ucarecdn.com/c354c00f-a972-4950-9e59-a8210caddebe/){ width=50% }

---

## Mermaid

![-](https://raw.githubusercontent.com/mermaid-js/mermaid/develop/docs/public/favicon.svg){ width=40% }

---

### Problema

![banco](./images/banco.svg){ width=70% }

---

### Bora pra prática!

![-](https://media1.giphy.com/media/HN6GLlUsMvue652b2w/giphy.gif?cid=ecf05e470bxv3gz929qe1ozwur1pjq5fzkpme6ac8j7lts6q&ep=v1_stickers_search&rid=giphy.gif&ct=s)


---

### Livros

![livros](./images/books.svg){ width=60% }

---

###### The software guidebook 

![The software guidebook](https://d2sofvawe08yqg.cloudfront.net/documenting-software-architecture/s_hero?1653735035)

---

###### The C4 model for visualising software architecture

![The C4 model for visualising software architecture](https://d2sofvawe08yqg.cloudfront.net/visualising-software-architecture/s_hero?1653735204)

---

#### Por onde começar?

![-](./images/faq.svg)

---

### Crie um bom Readme

---

### Crie seu Diagrama de Contexto

---

### De o primeiro passo
#### Documente!

---
