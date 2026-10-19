# Comandos do Windows para suporte

Abrir o Prompt de Comando (`cmd`). Os de reparo exigem **executar como administrador**.

## Rede

| Comando | Para que serve | O que olhar |
|---|---|---|
| `ipconfig` | Mostra o IP da máquina | Gateway padrão e IPv4. IP `169.254.x.x` = não pegou IP do roteador |
| `ipconfig /all` | Detalhes completos | DNS, MAC, DHCP ativo |
| `ping <gateway>` | Testa a rede local | Falhou: problema na rede local |
| `ping 8.8.8.8` | Testa se há internet | Enviados = Recebidos, 0% de perda = ok |
| `ping google.com` | Testa internet e DNS | Se o 8.8.8.8 responde e este não: problema de DNS |
| `ipconfig /flushdns` | Limpa o cache de DNS | Resolve sites que não abrem por cache velho |
| `ipconfig /release` e `/renew` | Solta e pede novo IP | Útil quando o IP está errado |

Leitura do `ping`: ele mostra se o destino **responde** e a latência (tempo de ida e volta, em ms; menor é melhor). Não mede a velocidade da internet.

### Ordem de diagnóstico de rede
1. `ipconfig`: tem IP e gateway?
2. `ping` no gateway: rede local ok?
3. `ping 8.8.8.8`: internet ok?
4. `ping google.com`: DNS ok?

## Sistema e disco

| Comando | Para que serve |
|---|---|
| `sfc /scannow` | Verifica e repara arquivos do Windows corrompidos (admin) |
| `chkdsk C: /f` | Verifica e corrige erros no disco; pede reiniciar (admin) |
| `tasklist` | Lista os processos, como o Gerenciador de Tarefas |
| `taskkill /PID 1234 /F` | Encerra um processo travado pelo número (PID) |
| `systeminfo` | Versão do Windows, RAM, tempo ligado |
| `hostname` | Nome da máquina |

### `sfc` ou `chkdsk`?
- `sfc`: arquivos do Windows com comportamento estranho.
- `chkdsk`: travamentos, lentidão ou suspeita de defeito no disco.
