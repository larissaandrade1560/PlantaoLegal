# Plantão Legal

## Visão geral

O Plantão Legal é um aplicativo acadêmico voltado para o controle de plantões, jornada de trabalho e horas extras. A proposta principal é ajudar profissionais com turnos irregulares a registrar sua carga horária de forma simples, privada e segura.

## Problema atendido

Profissionais de saúde e áreas operacionais costumam trabalhar em escalas alternadas, com plantões consecutivos e pouca disponibilidade para registrar horários com precisão. Isso dificulta o acompanhamento de horas trabalhadas, horas extras e descanso, aumentando o risco de fadiga e sobrecarga.

## Público-alvo

- médicos;
- enfermeiros;
- técnicos de enfermagem;
- seguranças;
- motoristas de aplicativo;
- bombeiros.

## Objetivo do projeto

O aplicativo deve permitir:

- registrar jornadas de trabalho rapidamente;
- calcular horas extras e carga horária;
- consultar histórico de plantões;
- visualizar um indicador de fadiga;
- gerar relatórios locais em PDF;
- manter funcionamento offline com privacidade.

## Principais funcionalidades

O protótipo contempla as seguintes funcionalidades:

- cadastro de plantões;
- registro de data e horários;
- cálculo da duração do plantão;
- acompanhamento de horas extras;
- consulta ao histórico;
- calendário de plantões;
- indicador de carga horária/fadiga;
- geração de relatórios;
- funcionamento offline.

---

## Protótipo

O projeto foi desenvolvido em duas etapas de prototipação:

### Baixa fidelidade

A baixa fidelidade foi utilizada para explorar a estrutura das telas, organização das informações e fluxo de navegação antes da definição visual final.

Arquivo:

`docs/prototipoBaixaFidelidade.pdf`

### Alta fidelidade

A alta fidelidade representa a proposta final da interface, incluindo identidade visual, cores, tipografia, componentes, informações, navegação e interações.

Arquivo:

`docs/prototipoAltaFidelidade.pdf`

---

## Fluxo principal

O fluxo principal do aplicativo contempla:

```text
Tela Inicial
     │
     ├── Novo Plantão
     │      ├── Data
     │      ├── Horário de início
     │      ├── Horário de término
     │      └── Salvar
     │
     ├── Histórico
     │      └── Calendário / Plantões
     │
     └── Relatórios
            └── Gerar relatório

## Participação individual

- Larissa Andrade — Liderança no projeto, definição do problema, requisitos, documentação, slides e prototipação.
- Matheus Costa — Apoio na definição e revisão das funcionalidades e suporte na prototipação, revisão da documentação.
- Gabriel Ramalho — Apoio na estrutura dos requisitos funcionais e do CRUD
- Genilson Dias — Apoio em requisitos não funcionais, privacidade, apoio nos requisitos referentes ao Github e apresentação do projeto.
- Hunald Barreto — Revisão final

## Estrutura do repositório

```text
PlantaoLegal/
├── README.md
├── CHANGELOG.md
├── docs/
│   ├── requisitos.md
│   └── apresentacaoRequisitos.pdf
└── .git/
```

## figma link
https://www.figma.com/design/eWMV2kegSIzYKbp38WpLS6/Prot%25C3%25B3tipo-2?node-id=0-1&p=f&t=EgHy22j4THG4Vvu1-0

```

## Observação

Este repositório foi ajustado para atender ao checklist da professora, incluindo requisitos mínimos, CRUD, priorização e documentação centralizada no arquivo de requisitos.
