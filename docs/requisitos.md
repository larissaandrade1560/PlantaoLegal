# Requisitos do Plantão Legal

## 1. Contexto e problema

O Plantão Legal foi pensado para atender profissionais que atuam em jornadas irregulares e plantões consecutivos, como médicos, enfermeiros, seguranças e motoristas de aplicativo. Esses usuários precisam controlar horas trabalhadas, horas extras e descanso, mas muitas vezes fazem isso de forma manual, incompleta ou pouco confiável. Esse cenário aumenta o risco de fadiga, sobrecarga e falhas na organização da rotina.

A proposta do aplicativo é reduzir essa dificuldade por meio de um registro simples e seguro das jornadas, com apoio visual para identificar carga horária e sinais de desgaste.

## 2. Funcionalidades principais

O aplicativo deve conter, no mínimo, as seguintes 8 funcionalidades principais:

1. Cadastro de plantão
2. Registro de data, início e término da jornada
3. Cálculo automático de duração do plantão
4. Cálculo de horas extras
5. Histórico de plantões
6. Indicador visual de fadiga em formato de bateria
7. Exportação de relatório em PDF
8. Alerta de descanso e carga horária elevada

Essas funcionalidades atendem diretamente ao problema principal do projeto e estão alinhadas com a proposta do estudo de caso e das personas.

## 3. Requisitos funcionais

### FR01 — Cadastro de plantão
O sistema deve permitir que o usuário cadastre um plantão informando data, horário de início e horário de término.

### FR02 — Cálculo automático de duração
O sistema deve calcular automaticamente a duração total do plantão com base no início e no término informados.

### FR03 — Validação de horários
O sistema deve impedir o cadastro de horários inválidos, como data inexistente, início maior que o fim ou jornadas impossíveis.

### FR04 — Registro de horas extras
O aplicativo deve identificar automaticamente as horas que excedem a jornada regular configurada.

### FR05 — Histórico de plantões
O sistema deve permitir a consulta do histórico de plantões realizados pelo usuário.

### FR06 — Filtro por período
O usuário deve poder consultar o histórico por data, semana ou mês.

### FR07 — Indicador de fadiga
O sistema deve exibir um indicador visual que represente a carga horária acumulada e a probabilidade de sobrecarga.

### FR08 — Alertas locais
O sistema deve emitir alertas locais quando houver carga elevada, registros pendentes ou necessidade de descanso.

### FR09 — Exportação de PDF
O usuário deve poder exportar relatórios em PDF a partir do histórico de plantões.

### FR10 — Armazenamento local das informações
O sistema deve salvar os dados do usuário no dispositivo para uso offline.

### FR11 — Edição de plantão
O usuário deve poder alterar informações de um plantão já cadastrado, caso seja necessário corrigir dados.

### FR12 — Exclusão de plantão
O usuário deve poder remover registros de plantões que não sejam mais relevantes.

## 4. Requisitos não funcionais

### RNF01 — Usabilidade
O usuário deve conseguir acessar a funcionalidade principal em, no máximo, três interações.

### RNF02 — Privacidade e segurança
Os dados do usuário devem ser armazenados localmente e protegidos contra acesso indevido.

### RNF03 — Offline
O aplicativo deve funcionar sem conexão ativa, especialmente em ambientes com sinal instável.

### RNF04 — Compatibilidade
A solução deve considerar Android 7.0 ou superior e funcionar em dispositivos com hardware intermediário.

### RNF05 — Acessibilidade
A interface deve priorizar contraste, legibilidade e uso confortável em ambiente noturno.

### RNF06 — Desempenho
O app deve responder rapidamente às ações principais, como cadastro, cálculo e consulta ao histórico.

## 5. Regras de segurança, privacidade e LGPD

O aplicativo deve respeitar os princípios de minimização, armazenamento local, transparência e controle do usuário. Informações sensíveis como horários, locais de trabalho e padrões de jornada devem ser mantidas no dispositivo, sem compartilhamento automático para servidores externos. A exportação de relatórios em PDF deve ocorrer somente mediante ação explícita do usuário.

## 6. CRUD

Quando aplicável, as operações de cadastro, leitura, atualização e exclusão devem estar previstas para o principal conjunto de dados do sistema.

| Entidade | C | R | U | D | Justificativa |
| --- | --- | --- | --- | --- | --- |
| Plantão | Sim | Sim | Sim | Sim | É a principal informação do sistema e precisa ser registrada, consultada, ajustada e removida quando necessário |
| Usuário | Sim | Sim | Sim | Não | O perfil do usuário é essencial para identificação e configuração, mas a exclusão completa pode não ser necessária na versão acadêmica |
| Relatório PDF | Sim | Sim | Não | Sim | O usuário pode gerar e remover relatórios locais, mas não precisa alterar o conteúdo do arquivo após a geração |
| Alerta de carga horária | Sim | Sim | Sim | Não | Os alertas podem ser gerados e visualizados, mas não exigem exclusão frequente na rotina |

A operação de exclusão de usuário pode ser dispensada na primeira versão, pois o escopo acadêmico prioriza o controle de jornada e não a gestão completa de identidade do usuário.

## 7. Priorização

### Essenciais
- Cadastro de plantão
- Cálculo de duração do plantão
- Cálculo de horas extras
- Histórico de plantões
- Exportação de relatório em PDF

### Importantes
- Indicador de fadiga
- Alertas locais
- Validação de horários
- Edição de plantão

### Secundárias
- Filtros por mês/semana
- Melhorias de acessibilidade visual
- Ajustes avançados de notificação

## 8. Relação com problema, pesquisa e personas

As funcionalidades e requisitos foram definidos para atender diretamente ao problema central do projeto: a dificuldade de controlar jornadas e evitar sobrecarga. Elas também dialogam com a pesquisa e com as personas, especialmente em relação à necessidade de rapidez, uso em condições de cansaço, privacidade e operação offline.

## 9. Conclusão

O Plantão Legal deve ser uma solução simples, prática e segura para monitorar turnos e horas extras. A sua proposta principal é facilitar o acompanhamento da jornada sem exigir muito esforço do usuário, protegendo dados pessoais e oferecendo suporte para a prevenção de fadiga e sobrecarga.

A entrega final deve manter foco nas funcionalidades essenciais, nos requisitos funcionais e nos critérios de qualidade que sustentam a proposta do aplicativo.
