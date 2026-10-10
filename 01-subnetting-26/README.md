# Network Labs

Exercícios de redes feitos no Cisco Packet Tracer, durante a formação em Cibersegurança.

---

## 01 - Subnetting /26

Exercício de aula: dividir uma rede /24 em 4 sub-redes /26.

### Plano de endereçamento

| Rede | Sub-rede | Broadcast | Hosts úteis |
|---|---|---|---|
| Rede 1 | 200.20.20.0 | 200.20.20.63 | .1 a .62 |
| Rede 2 | 200.20.20.64 | 200.20.20.127 | .65 a .126 |
| Rede 3 | 200.20.20.128 | 200.20.20.191 | .129 a .190 |
| Rede 4 | 200.20.20.192 | 200.20.20.255 | .193 a .254 |

Máscara: 255.255.255.192 (/26). Cada bloco tem 64 endereços (2⁶), dos quais 62 são úteis.

### Topologia

![Topologia](01-subnetting-26/imagens/topologia.png)

### Configuração IP (exemplo: PC4)

![IP do PC4](01-subnetting-26/imagens/ip-pc4.png)

### Testes de conectividade

![Ping do PC4](01-subnetting-26/imagens/ping-pc4.png)

- Ping dentro da mesma rede (.66 e .68): **funciona**.
- Ping para outras redes (.129 e .1): **falha**, porque não há router nem gateway configurado.

### O que aprendi

(escreve aqui, por palavras tuas, porque é que o PC4 não chega às outras redes)

Ficheiro do Packet Tracer: [`subnetting-26.pkt`](01-subnetting-26/subnetting-26.pkt)

---

## 02 - Subnetting /25

Em preparação.
