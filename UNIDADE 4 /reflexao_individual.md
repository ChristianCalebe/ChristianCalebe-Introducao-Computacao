# Reflexão Individual – Aula 11

> **Pergunta norteadora:** *"Qual topologia seria mais adequada para a rede da minha residência e por quê?"*

---

### Análise das Topologias Alternativas

Para entender a melhor escolha, é preciso primeiro descartar as opções que não se adequam à realidade de uma casa:

* **Topologia em Barramento:** Historicamente baseada em cabos coaxiais, essa arquitetura compartilha o mesmo meio físico para todos os equipamentos. Em uma casa, seria um desastre: além da lentidão gerada pelo excesso de colisões de dados, um simples rompimento no cabo principal deixaria toda a família sem internet. Hoje, é uma tecnologia em desuso.
* **Topologia em Anel:** Funciona através da passagem de um *"token"* (ficha) no circuito. O grande problema para o uso doméstico é a interdependência: se um computador do anel for desligado ou apresentar defeito, o ciclo se quebra e a rede cai. Além disso, adicionar um novo celular ou notebook exigiria parar o funcionamento da rede, o que é inviável no dia a dia.
* **Topologia em Malha (Mesh):** Oferece o mais alto nível de redundância, pois todos os pontos se conectam entre si. No entanto, o excesso de cabos e o custo elevadíssimo dos equipamentos necessários tornam essa opção um verdadeiro exagero para uma casa. Ela é perfeita para *data centers*, mas desnecessária para uma rede residencial básica.

---

### Topologia Recomendada: Estrela

Para o cenário doméstico, a **topologia em estrela** é a escolha ideal e definitiva. Nesse modelo, todos os dispositivos (smartphones, televisores, videogames, etc.) não se conectam diretamente entre si, mas sim a um nó centralizador — que, nas nossas casas, é o modem/roteador Wi-Fi fornecido pela operadora (ou adquirido à parte).

#### Principais vantagens que justificam essa escolha:

1. **Resiliência a falhas individuais:** Se o cabo do computador quebrar ou a placa de rede da Smart TV queimar, apenas aquele dispositivo perde a conexão. O resto da casa continua navegando perfeitamente.
2. **Escalabilidade e praticidade:** É extremamente simples expandir a rede. Para adicionar um novo dispositivo (*host*), basta conectá-lo via cabo em uma porta livre do roteador ou inserir a senha do Wi-Fi, sem precisar reconfigurar ou paralisar os outros aparelhos.
3. **Economia:** Os equipamentos baseados nessa topologia (switches e roteadores domésticos) são produzidos em massa, o que torna o custo de implementação baixíssimo.
4. **Tráfego otimizado:** Como cada aparelho tem uma via dedicada até o roteador central, as colisões de pac
