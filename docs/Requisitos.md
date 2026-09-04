# Requisitos Funcionais

## 5.1 Estação

**RF01 — Cadastro da estação**

> O sistema deve permitir o cadastro de uma estação de beleza.
> 

**RF02 — Registro dos dados da estação**

> O sistema deve permitir o registro das informações necessárias para identificação e funcionamento da estação.
> 

**RF03 — Consulta dos dados da estação**

> O sistema deve permitir que usuários autorizados consultem os dados da estação.
> 

**RF04 — Atualização dos dados da estação**

> O sistema deve permitir que usuários autorizados atualizem os dados cadastrados.
> 

**RF05 — Ativação e desativação da estação**

> O sistema deve permitir controlar o status da estação.
> 

---

# 5.2 Usuários e acesso

**RF06 — Cadastro de usuário**

> O sistema deve permitir que usuários autorizados cadastrem novos usuários vinculados à estação.
> 

**RF07 — Definição do perfil**

> O sistema deve permitir definir o perfil de cada usuário.
> 

Perfis iniciais:

```
Proprietário/Gestor
Atendente
Profissional
```

**RF08 — Autenticação**

> O sistema deve permitir que usuários cadastrados realizem autenticação.
> 

**RF09 — Consulta de usuários**

> O sistema deve permitir que usuários autorizados consultem os usuários vinculados à estação.
> 

**RF10 — Atualização de usuário**

> O sistema deve permitir que usuários autorizados atualizem os dados de usuários.
> 

**RF11 — Ativação e desativação de usuário**

> O sistema deve permitir ativar ou desativar usuários.
> 

**RF12 — Controle de acesso**

> O sistema deve controlar o acesso às funcionalidades de acordo com o perfil e permissões do usuário.
> 

---

# 5.3 Clientes

**RF13 — Cadastro de cliente**

> O sistema deve permitir cadastrar clientes vinculados à estação.
> 

**RF14 — Registro dos dados do cliente**

> O sistema deve permitir registrar as informações necessárias para identificação e atendimento.
> 

**RF15 — Consulta de clientes**

> O sistema deve permitir consultar clientes cadastrados.
> 

**RF16 — Busca de clientes**

> O sistema deve permitir localizar clientes por informações de identificação.
> 

**RF17 — Atualização de cliente**

> O sistema deve permitir atualizar os dados de um cliente.
> 

**RF18 — Histórico do cliente**

> O sistema deve permitir consultar o histórico de atendimentos e serviços realizados.
> 

**RF19 — Ativação e desativação de cliente**

> O sistema deve permitir ativar ou desativar um cliente.
> 

---

# 5.4 Profissionais

**RF20 — Cadastro de profissional**

> O sistema deve permitir cadastrar profissionais vinculados à estação.
> 

**RF21 — Registro dos dados do profissional**

> O sistema deve permitir registrar as informações necessárias para identificação e atuação do profissional.
> 

**RF22 — Consulta de profissionais**

> O sistema deve permitir consultar profissionais cadastrados.
> 

**RF23 — Atualização de profissional**

> O sistema deve permitir atualizar os dados de um profissional.
> 

**RF24 — Associação de profissional a serviços**

> O sistema deve permitir associar serviços aos profissionais habilitados a realizá-los.
> 

**RF25 — Definição da disponibilidade**

> O sistema deve permitir configurar os períodos de disponibilidade de cada profissional.
> 

**RF26 — Ativação e desativação**

> O sistema deve permitir ativar ou desativar profissionais.
> 

**RF27 — Consulta da agenda**

> O sistema deve permitir que usuários autorizados consultem os agendamentos relacionados aos profissionais.
> 

---

# 5.5 Serviços

**RF28 — Cadastro de serviço**

> O sistema deve permitir cadastrar serviços oferecidos pelos profissionais da estação.
> 

**RF29 — Registro dos dados do serviço**

> O sistema deve permitir registrar as informações necessárias para realização do serviço.
> 

**RF30 — Definição do preço**

> O sistema deve permitir definir o preço do serviço.
> 

**RF31 — Definição da duração**

> O sistema deve permitir definir a duração estimada do serviço.
> 

**RF32 — Consulta de serviços**

> O sistema deve permitir consultar serviços cadastrados.
> 

**RF33 — Atualização de serviço**

> O sistema deve permitir atualizar os dados de um serviço.
> 

**RF34 — Associação de serviço a profissional**

> O sistema deve permitir associar serviços aos profissionais que os realizam.
> 

**RF35 — Ativação e desativação**

> O sistema deve permitir ativar ou desativar serviços.
> 

---

# 5.6 Agenda e agendamentos

Este continua sendo o **coração do MVP**.

**RF36 — Visualização da agenda**

> O sistema deve permitir visualizar a agenda da estação.
> 

**RF37 — Visualização por profissional**

> O sistema deve permitir visualizar a agenda individual de cada profissional.
> 

**RF38 — Visualização por período**

> O sistema deve permitir visualizar agendamentos por diferentes períodos.
> 

**RF39 — Identificação do status**

> O sistema deve apresentar o status de cada agendamento.
> 

**RF40 — Criação de agendamento**

> O sistema deve permitir criar agendamentos.
> 

**RF41 — Seleção do cliente**

> O sistema deve permitir associar um cliente ao agendamento.
> 

**RF42 — Seleção do serviço**

> O sistema deve permitir selecionar o serviço.
> 

**RF43 — Seleção do profissional**

> O sistema deve permitir selecionar o profissional responsável.
> 

**RF44 — Definição de data e horário**

> O sistema deve permitir definir data e horário.
> 

**RF45 — Verificação de disponibilidade**

> O sistema deve verificar a disponibilidade do profissional.
> 

**RF46 — Prevenção de conflitos**

> O sistema deve impedir conflitos de horários.
> 

**RF47 — Alteração de agendamento**

> O sistema deve permitir alterar agendamentos conforme as permissões do usuário.
> 

**RF48 — Cancelamento**

> O sistema deve permitir cancelar agendamentos conforme as permissões do usuário.
> 

**RF49 — Remarcação**

> O sistema deve permitir remarcar agendamentos.
> 

**RF50 — Consulta**

> O sistema deve permitir consultar agendamentos.
> 

**RF51 — Busca**

> O sistema deve permitir buscar agendamentos.
> 

---

# 5.7 Financeiro individual do profissional

Essa é uma **nova área decorrente do modelo de estação**.

**RF52 — Registro de ganhos**

> O sistema deve permitir registrar os ganhos relacionados aos atendimentos do profissional.
> 

**RF53 — Consulta dos ganhos**

> O profissional deve poder consultar seus próprios ganhos.
> 

**RF54 — Histórico financeiro individual**

> O sistema deve permitir consultar o histórico financeiro individual do profissional.
> 

**RF55 — Isolamento financeiro**

> O sistema deve impedir que um profissional consulte os dados financeiros de outro profissional.
> 

> **Observação:** o escopo exato do financeiro do MVP ainda deve ser definido. Não estamos transformando o sistema em um ERP financeiro completo.
> 

---

# 5.8 Controle de aluguel/espaço

Outra funcionalidade derivada do modelo de estação.

**RF56 — Registro do aluguel do profissional**

> O sistema deve permitir registrar informações relacionadas ao aluguel ou utilização do espaço pelo profissional.
> 

**RF57 — Vencimento**

> O sistema deve permitir registrar a data de vencimento do aluguel.
> 

**RF58 — Consulta de vencimentos**

> O proprietário deve poder consultar os vencimentos dos profissionais.
> 

**RF59 — Status do aluguel**

> O sistema deve permitir identificar a situação do aluguel.
>

# Requisitos Não Funcionais

**RNF01 — Autenticação segura**

**RNF02 — Proteção de credenciais**

**RNF03 — Controle de acesso**

**RNF04 — Isolamento dos dados da estação**

**RNF05 — Isolamento dos dados individuais dos profissionais**

**RNF06 — Proteção de dados pessoais**

**RNF07 — Conformidade com legislação aplicável**

**RNF08 — Tempo de resposta**

**RNF09 — Eficiência das operações de agenda**

**RNF10 — Disponibilidade**

**RNF11 — Interface intuitiva**

**RNF12 — Responsividade**

**RNF13 — Escalabilidade**

**RNF14 — Manutenibilidade**

**RNF15 — Modularidade**

**RNF16 — Compatibilidade com navegadores**

**RNF17 — Integridade dos dados**