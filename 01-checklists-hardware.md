# Checklists de hardware

Regra geral: do mais simples e barato para o mais específico. Testar uma coisa por vez.

## 1. Computador não liga

### 1.1 Sem sinal de vida (sem LED, sem ventoinha)

| # | Passo | O que verificar | O que indica |
|---|---|---|---|
| 1 | Tomada | Testar em outra tomada ou com outro aparelho | Tomada sem energia |
| 2 | Cabo de energia | Trocar o cabo | Cabo defeituoso |
| 3 | Chave da fonte | Posição ON/OFF (I/O) | Fonte desligada na chave |
| 4 | Periféricos | Remover USBs e outros dispositivos | Dispositivo causando curto |
| 5 | Cabos da fonte na placa | 24 pinos e CPU bem encaixados | Mau contato |
| 6 | Fonte | Testar com outra fonte | Fonte queimada |

### 1.2 Liga, mas sem imagem

| # | Passo | O que verificar | O que indica |
|---|---|---|---|
| 1 | Cabo de vídeo | HDMI/DisplayPort firmes, entrada certa do monitor | Cabo ruim ou entrada errada |
| 2 | Saída de vídeo | Cabo na placa de vídeo, não na placa-mãe | Imagem some na saída errada |
| 3 | Memória RAM | Reencaixar e testar um pente por vez, em outro slot | Pente ou slot defeituoso |
| 4 | Placa de vídeo | Reencaixar no slot | Mau contato |
| 5 | Bipes e LEDs | Código de bipes da placa-mãe | Aponta RAM, vídeo ou CPU |
| 6 | CMOS | Limpar ou trocar a bateria | BIOS desconfigurada |

### 1.3 Mostra tela, mas não inicia o Windows

| # | Passo | O que verificar | O que indica |
|---|---|---|---|
| 1 | Mensagem na tela | "No bootable device", "Operating system not found" | Sistema não encontra o disco |
| 2 | BIOS | O SSD aparece na lista de discos? | Se não aparece, problema físico |
| 3 | Ordem de boot | Disco do sistema como primeiro | Boot em dispositivo errado |
| 4 | Cabos do SSD | Dados e energia bem encaixados | Mau contato |
| 5 | Reparo de inicialização | Mídia do Windows, "Reparar o computador" | Sistema corrompido |
| 6 | Saúde do disco | SMART / teste do fabricante | Disco falhando; fazer backup e trocar |

## 2. Computador lento

| # | Passo | O que verificar | O que indica |
|---|---|---|---|
| 1 | Gerenciador de Tarefas | Processo usando CPU, RAM ou disco em excesso | Programa travado ou pesado |
| 2 | Desempenho | CPU, RAM, disco e rede entregando o esperado | Componente no limite (gargalo) |
| 3 | Temperatura | Temperatura de CPU e demais componentes | Superaquecimento reduz o desempenho (thermal throttling) |
| 4 | Cooler e pasta térmica | Cooler conectado e girando; pasta térmica velha | Refrigeração falha; trocar a pasta |
| 5 | Espaço livre no SSD | Pouco espaço livre | Trava e lentidão |
| 6 | Limpeza | Limpeza de disco, arquivos temporários e cache | Disco cheio de lixo |
| 7 | Inicialização | Itens que abrem com o Windows | Desativar o que for desnecessário |
| 8 | Vírus e malware | Varredura completa | Causa clássica de lentidão |
| 9 | Atualizações | Windows e drivers | Falhas e incompatibilidades corrigidas |
