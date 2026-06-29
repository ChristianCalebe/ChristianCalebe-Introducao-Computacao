# Reflexão Individual – Aula 11

**Nome:** [Christian Calebe Ferreira Campos Silva]
**Matrícula:** [22611286]
**Disciplina:** Introdução à Computação

*"Qual topologia seria mais adequada para a rede da minha residência e por quê?"*

## 1. Avaliação Crítica das Alternativas Estruturais

A seleção de uma arquitetura de rede para ambientes domésticos exige a ponderação entre custos, complexidade de gestão e tolerância a falhas. Abaixo, analisam-se as abordagens tradicionais e os seus respetivos impactos se aplicadas a um contexto residencial moderno:

| Topologia | Mecanismo e Características | Viabilidade Residencial |
| :--- | :--- | :--- |
| **Barramento (Bus)** | Utiliza um canal físico central partilhado (linear) no qual todos os nós se ligam. | **Inviável.** Apresenta um alto índice de colisão de pacotes e vulnerabilidade total: se o cabo principal falhar, todo o sistema fica inoperacional. Tecnicamente obsoleta. |
| **Anel (Ring)** | Os nós ligam-se em circuito fechado. Os dados circulam sequencialmente por meio de uma permissão digital (token). | **Inadequada.** Qualquer quebra física no circuito ou desligamento de um nó interrompe o fluxo geral. A expansão exige pausas temporárias na rede. |
| **Malha (Mesh)** | Implementa ligações diretas ponto a ponto redundantes entre todos os dispositivos. | **Incompatível.** Embora seja extremamente resiliente, o custo e o volume de cablagem ou configurações são excessivos para o ambiente doméstico. |

## 2. Recomendação Técnica: Topologia em Estrela

Para atender com eficiência às exigências residenciais contemporâneas, a **Topologia em Estrela** estabelece-se como a escolha ideal. Nesta configuração, cada dispositivo (seja computador, consola, smart TV ou smartphone) mantém um canal de comunicação individual focado num único elemento centralizador, papel desempenhado no quotidiano pelos routers domésticos.

Os critérios técnicos que fundamentam esta recomendação incluem:

* **Segregação de Incidentes:** Caso ocorra uma rutura de cabo ou falha de hardware num equipamento específico, o impacto fica estritamente restrito àquele ponto. O restante da rede permanece ativo, diferenciando-se crucialmente dos modelos em barramento ou anel.
* **Escalabilidade Dinâmica (Plug-and-Play):** A introdução ou remoção de novos componentes é executada de forma independente. Não há interrupção do sinal dos demais utilizadores ao ligar um cabo ou associar um aparelho ao Wi-Fi.
* **Sustentabilidade Financeira:** A infraestrutura central necessária é altamente acessível. Os routers de consumo atual reúnem funções de modem, switch e ponto de acesso numa única peça de custo moderado.
* **Otimização de Desempenho Local:** Devido aos canais de comunicação exclusivos criados entre a central e os dispositivos, mitiga-se o problema de colisões físicas de dados.
* **Nativa com Padrões Atuais:** Os protocolos dominantes do mercado — como a cablagem Ethernet (Cat6) e as redes sem fios de última geração (Wi-Fi 6) — são concebidos intrinsecamente para operar sob a lógica concêntrica da estrela.

## 3. Mapeamento do Cenário Prático

Num ambiente de uso real moderno, a materialização desta topologia ocorre através da receção do sinal de internet por fibra ótica de alta velocidade (padrão FTTH) que alimenta diretamente o router central. Este núcleo inteligente atua como o distribuidor concêntrico da residência.

A distribuição é dividida estrategicamente em dois eixos secundários a partir da estrela: o segmento sem fios (frequências de 5 GHz ou 6 GHz do Wi-Fi) providencia mobilidade fluida a telemóveis e portáteis; em paralelo, portas cabladas Ethernet de alta capacidade ligam diretamente os equipamentos que exigem estabilidade e velocidade contínua, como computadores de trabalho e smart TVs.

## Conclusão

A arquitetura em estrela representa a melhor convergência entre segurança operacional, facilidade de expansão e custo de implementação para o cenário residencial. Enquanto alternativas como malhas completas ou circuitos em anel encontram o seu propósito em infraestruturas industriais e centros de dados de missão crítica, a simplicidade resiliente da estrela consolida-a como o padrão soberano para o utilizador doméstico final.
