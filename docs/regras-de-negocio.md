# Regras de negócio

## Estação

**RN01 — Isolamento entre estações**

Cada estação deve possuir seus próprios usuários, clientes, profissionais, serviços e agendamentos.

**RN02 — Estação ativa**

Somente estações ativas poderão utilizar as funcionalidades operacionais.

**RN03 — Desativação da estação**

A desativação não deverá apagar automaticamente seu histórico.

---

## Usuários

**RN04 — Usuário vinculado à estação**

Um usuário operacional deve estar vinculado a uma estação.

**RN05 — Perfil do usuário**

Cada usuário deve possuir um perfil que determine suas permissões.

**RN06 — Acesso conforme permissão**

Um usuário somente poderá executar operações autorizadas.

**RN07 — Usuário desativado**

Usuários desativados não poderão realizar autenticação.

**RN08 — Proprietário inicial**

O usuário responsável pela criação da estação será associado inicialmente ao perfil Proprietário/Gestor.

---

## Clientes

**RN09 — Cliente vinculado à estação**

Um cliente deve pertencer a uma estação.

**RN10 — Prevenção de duplicidade**

O sistema deve possuir mecanismos para evitar cadastros duplicados.

**RN11 — Histórico**

Os atendimentos devem permanecer vinculados ao histórico do cliente.

**RN12 — Desativação**

A desativação do cliente não deverá apagar seu histórico.

---

## Profissionais

**RN13 — Profissional vinculado à estação**

Um profissional deve estar associado a uma estação.

**RN14 — Profissional ativo**

Somente profissionais ativos poderão receber novos agendamentos.

**RN15 — Serviços do profissional**

O profissional somente poderá receber agendamentos para serviços aos quais esteja associado.

**RN16 — Disponibilidade**

Agendamentos devem respeitar a disponibilidade do profissional.

**RN17 — Isolamento financeiro**

Um profissional não poderá acessar informações financeiras de outro profissional.

---

# Agendamentos

**RN18 — Informações obrigatórias**

Um agendamento deve possuir cliente, profissional, serviço, data e horário.

**RN19 — Profissional disponível**

O profissional deve estar disponível no período solicitado.

**RN20 — Prevenção de conflitos**

Não poderá existir sobreposição entre agendamentos ativos do mesmo profissional.

**RN21 — Duração do serviço**

A duração do serviço deve ser considerada no cálculo de disponibilidade.

**RN22 — Profissional habilitado**

O profissional deve estar associado ao serviço escolhido.

**RN23 — Profissional inativo**

Não poderão ser criados novos agendamentos para profissionais inativos.

**RN24 — Serviço inativo**

Não poderão ser criados novos agendamentos para serviços inativos.

**RN25 — Alteração**

Alterações devem passar novamente pelas regras de disponibilidade e conflito.

**RN26 — Remarcação**

A remarcação somente poderá ocorrer se o novo horário estiver disponível.

**RN27 — Cancelamento**

Um agendamento cancelado não deve continuar ocupando a agenda.

**RN28 — Histórico**

Agendamentos realizados devem preservar informações relevantes mesmo após conclusão ou cancelamento.

---

# Permissões da agenda

Essa foi uma decisão importante tomada durante a revisão.

| Ação | Proprietário | Atendente | Profissional |
| --- | --- | --- | --- |
| Criar agendamento | ✅ | ✅ | ✅ |
| Consultar agenda | ✅ | ✅ | ✅ |
| Alterar próprio agendamento | ✅ | ✅ | ✅ |
| Alterar agendamento de outro profissional | ✅ | ✅ | ❌ |
| Cancelar próprio agendamento | ✅ | ✅ | ✅ |
| Cancelar agendamento de outro profissional | ✅ | ✅ | ❌ |
| Gerenciar agenda da estação | ✅ | ✅ | ❌ |

### RN29 — Gestão central da agenda

> O atendente poderá gerenciar os agendamentos dos diferentes profissionais da estação.
> 

### RN30 — Autonomia do profissional

> O profissional poderá criar, consultar, alterar e cancelar seus próprios agendamentos.
> 

### RN31 — Limitação do profissional

> O profissional não poderá alterar ou cancelar diretamente os agendamentos pertencentes a outro profissional.
> 

---

# Cancelamento

**RN32 — Cancelamento solicitado pelo profissional**

> O profissional poderá cancelar seus próprios agendamentos conforme as regras estabelecidas pela estação.
> 

**RN33 — Cancelamento pela atendente**

> A atendente poderá cancelar agendamentos de qualquer profissional da estação.
> 

**RN34 — Registro do cancelamento**

> O sistema deverá preservar informações relevantes sobre o cancelamento, incluindo, quando aplicável, quem realizou a ação e o motivo informado.
> 

**RN35 — Notificação do cliente**

> Quando um agendamento for cancelado, o sistema deverá permitir futuramente que o cliente seja comunicado sobre o cancelamento.
> 

**Observação:** a automação de notificações poderá ficar fora do MVP inicial.

---

# Operação

**RN36 — Horário de funcionamento**

Os agendamentos devem respeitar o horário de funcionamento da estação.

**RN37 — Disponibilidade do profissional**

A disponibilidade individual do profissional também deve ser considerada.

**RN38 — Períodos indisponíveis**

Períodos bloqueados não poderão receber novos agendamentos.

---

# Histórico

**RN39 — Conclusão do atendimento**

Um agendamento poderá ser marcado como concluído após a realização do serviço.

**RN40 — Histórico do cliente**

Um atendimento concluído deverá compor o histórico do cliente.

**RN41 — Valor histórico**

O valor praticado no momento do atendimento deve ser preservado.

**RN42 — Preservação histórica**

Alterações posteriores no cadastro do serviço não devem alterar automaticamente informações históricas.