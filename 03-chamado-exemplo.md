# Chamados, SLA e níveis de suporte

## Conceitos

**Chamado (ticket):** registro formal de um incidente (problema) ou requisição (pedido de acesso, instalação etc.), com número, histórico e responsável.

**SLA (Service Level Agreement):** prazo combinado para atender e resolver um chamado, conforme a prioridade.

| Prioridade | Exemplo | Primeiro atendimento | Resolução |
|---|---|---|---|
| Crítica | Servidor parado, empresa sem trabalhar | 15 min | 2 h |
| Alta | Setor sem sistema; usuário sem máquina | 1 h | 4 h |
| Média | Um usuário sem acesso a um sistema | 4 h | 1 dia útil |
| Baixa | Instalar programa, dúvida | 1 dia | 3 dias úteis |

A prioridade vem do **impacto** (quantos e quanto param) e da **urgência**. Os prazos acima são um exemplo; cada empresa define os seus.

**Níveis de suporte**

| Nível | Quem atende | Exemplos |
|---|---|---|
| N1 | Primeiro contato | Reiniciar, trocar cabo/peça, reset de senha, instalar programa |
| N2 | Técnico mais experiente | Rede, equipamentos, Active Directory, ERP |
| N3 | Especialista / infraestrutura | Servidores, banco de dados, segurança, fornecedor |

Escalar = passar o chamado ao próximo nível **registrando o que já foi testado**. Prioridade (a pressa) e nível (quem resolve) são independentes.

## Modelo de chamado

```
Chamado Nº:            Aberto:            Fechado:
Solicitante / Setor / Ramal:
Equipamento (patrimônio):
Descrição do problema:
Quando começou:
O que já foi tentado:
Impacto (impede de trabalhar?):
Prioridade:        Nível:
Diagnóstico (passos e resultado de cada um):
Solução aplicada:
Status:
```

## Exemplo preenchido: liga, mas sem vídeo

```
Chamado Nº: 0001
Solicitante: Lincoln - TI - ramal 5109
Equipamento: Desktop PAT-0142
Descrição: Computador liga, mas não sobe vídeo.
Sintoma observado: ventoinhas giram e há LED aceso; sem imagem no monitor.
Quando começou: Hoje de manhã; ontem funcionava normalmente.
Já tentado: troca de tomada e cabo de energia.
Impacto: impede o trabalho (sem máquina reserva).
Prioridade: Alta     Nível: N1
Diagnóstico:
  1. Tomada, cabo e chave da fonte: sem mudança.
  2. Reencaixe e limpeza da memória RAM: sem mudança.
  3. Troca do pente de RAM: o computador ligou.
  4. Pente antigo testado em outro slot: continuou sem vídeo (defeito no pente, não no slot).
Solução: substituição do pente de RAM (defeituoso).
Status: Concluído, confirmado pelo usuário.
```

> Chamado de exemplo para fins de estudo; patrimônio e ramal são fictícios.
