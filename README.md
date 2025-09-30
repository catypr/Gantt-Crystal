# Grafico-Gannt
```mermaid
flowchart TD

A(["Inicio"])
A--> B{"Faça uma escolha"}
B--> C["OP1"]
B--> D["OP2"]
B--> E["OP3"]
```

```mermaid
graph TD;
A[Inicio]-->B{Nota >6};
B--> |SIM| C[Aprovado];
B--> |NÃO| D[Reprovado];
```

```mermaid
gantt
title Exemplo de Gráfico de Gantt
dateFormat YYYY-MM-DD
section 1ºSemestre
1ºBimestre Finalizado:done, a1, 2025-02-02, 60d
2ºBimestre Finalizado:done, a2, after a1, 60d
section 2ºSemestre
3ºBimestre Em Andamento:active, a3, 2025-08-01, 60d
4ºBimestre Em Andamento:crit, a4, after a3, 60d
```


# Grafico-Gannt-Atividade
```mermaid
gantt
title Construção de Casa
dateFormat YYYY-MM-DD
section Início do Projeto
Planejamentos e Aprovações: done, a1, 2025-05-01, 20d
Preparação do Terreno: active, a2, after a1, 10d
Construção da Casa: crit, a3, after a2, 15d
Fundação: crit, a4, after a3, 30d
Instalção Elétrica e Hidráulica: crit, a5, after a4, 20d
Acabamento Interno: crit, a6, after a5, 25d
Acabento Externo: crit, a7, after a6, 15d
section Final do Projeto
Inspeção Final e Entrega da Casa: crit, a8, after a7, 5d
```

# Metodo-Agil-Crystal
```mermaid
graph TD
 subgraph Exercício 01
  A1["Conforto 8"]:::branco --> A2["D20"]:::amarelo --> A3["E50"]:::laranja --> A4["V100"]:::vermelho
    B1["C8"]:::branco --> B2["Essencial 20"]:::amarelo --> B3["E50"]:::laranja --> B4["V100"]:::vermelho
    C1["C8"]:::branco --> C2["D20"]:::amarelo --> C3["E50"]:::laranja --> C4["Vida 100"]:::vermelho
    D1["C8"]:::branco --> D2["Dinheiro 20"]:::amarelo --> D3["E50"]:::laranja --> D4["V100"]:::vermelho
    E1["C8"]:::branco --> E2["D20"]:::amarelo --> E3["Conforto 50"]:::laranja --> E4["V100"]:::vermelho
    F1["C8"]:::branco --> F2["Dinheiro 20"]:::amarelo --> F3["E50"]:::laranja --> F4["V100"]:::vermelho
    G1["C8"]:::branco --> G2["D20"]:::amarelo --> G3["E50"]:::laranja --> G4["Vida 100"]:::vermelho
    H1["C8"]:::branco --> H2["D20"]:::amarelo --> H3["E50"]:::laranja --> H4["Essencial 100"]:::vermelho
  end
 
  %% Definições de estilo
  classDef branco fill:#ffffff,stroke:#000,stroke-width:1px;
  classDef amarelo fill:#FFD80D,stroke:#000,stroke-width:1px;
  classDef laranja fill:#FFA233,stroke:#000,stroke-width:1px;
  classDef vermelho fill:#E64C3C,stroke:#000,stroke-width:1px;
 
```

```mermaid
graph TD
  subgraph Exercício 02
    A1["Conforto 8"]:::branco --> A2["D20"]:::amarelo --> A3["E50"]:::laranja --> A4["V100"]:::vermelho
    B1["C8"]:::branco --> B2["Essencial 20"]:::amarelo --> B3["E50"]:::laranja --> B4["V100"]:::vermelho
    C1["C8"]:::branco --> C2["D20"]:::amarelo --> C3["E50"]:::laranja --> C4["Vida100"]:::vermelho
    D1["Conforto 8"]:::branco --> D2["D20"]:::amarelo --> D3["E50"]:::laranja --> D4["V100"]:::vermelho
    E1["Dinheiro 8"]:::branco --> E2["D20"]:::amarelo --> E3["E50"]:::laranja --> E4["V100"]:::vermelho
    F1["C8"]:::branco --> F2["D20"]:::amarelo --> F3["Essencial 50"]:::laranja --> F4["V100"]:::vermelho
    G1["C8"]:::branco --> G2["D20"]:::amarelo --> G3["Dinheiro 50"]:::laranja --> G4["V100"]:::vermelho
    H1["C8"]:::branco --> H2["D20"]:::amarelo --> H3["E50"]:::laranja --> H4["Vida 100"]:::vermelho
  end
 
  %% Definições de estilo
  classDef branco fill:#ffffff,stroke:#000,stroke-width:1px;
  classDef amarelo fill:#FFD80D,stroke:#000,stroke-width:1px;
  classDef laranja fill:#FFA233,stroke:#000,stroke-width:1px;
  classDef vermelho fill:#E64C3C,stroke:#000,stroke-width:1px;

```

# Gantt - Avaliativa / Sistema de Cadastro de Empresas Parceiras
``` mermaid
gantt
title Sistema de Cadastro de Empresas Parceiras
dateFormat YYYY-MM-DD
section Inicio do Projeto
Configuração do Ambiente de Desenvolvimento: crit, a1, 2025-02-01, 15d
Criação do Banco de Dados: crit, a2, after a1, 15d
Programação do Módulo de Login: crit, a3, after a2, 20d
Programação do CRUD de Empresas: crit, a4, after a3, 20d
Implementação do Upload de Logotipo: crit, a5, after a4, 20d
Desenvolvimento dos Relatórios: crit, a6, after a5, 15d
Configuração do Painel Administrativo: crit, a7, after a6, 20d
Testes Unitários e de Integração: crit, a8, after a7, 15d
section Final do Projeto
Testes de Usabilidade com Usuários Convidados: crit, a9, after a8, 15d
Implementação Final no Servidor e Entrega ao Cliente: a10, after a9, 20d
```

# Metodo-Agil-Crystal / Sistema de Cadastro de Empresas Parceiras
```mermaid
graph TD
   subgraph Entrega 
     A1["Entrega 1 C8"]:::branco
     A2["Entrega 2 E100"]:::vermelho
     A3["Enterga 3 E20"]:::amarelo
     A4["Entrega 4 E8"]:::amarelo
     A5["Entrega 5 E50"]:::laranja
     A6["Entrega Final E100"]:::vermelho

A1 --> A2 --> A3 --> A4 --> A5 --> A6 
end

%% Definição de estilo
classDef branco fill:#ffffff, stroke:#000,stroke-width:1px;
classDef amarelo fill:#FFD80D, stroke:#000,stroke-width:1px;
classDef laranja fill:#FFA233, stroke:#000,stroke-width:1px;
classDef vermelho fill:#E64C3C, stroke:#000,stroke-width:1px;
```
