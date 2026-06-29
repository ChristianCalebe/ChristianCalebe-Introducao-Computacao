# Trabalho Prático: Conceitos, Atributos e Ameaças à Segurança da Informação

**Aula:** 14 – Segurança da Informação  

  # 1. Conceitos Fundamentais da Segurança da Informação

## Definição Formal (ISO/IEC 27000:2018)
Segundo a norma internacional **ISO/IEC 27000:2018** (que fundamenta a família 27000 de gestão de segurança), a **Segurança da Informação** é definida como:

> *"A preservação da confidencialidade, integridade e disponibilidade da informação. Adicionalmente, outras propriedades, tais como autenticidade, responsabilidade, não repúdio e confiabilidade, podem também estar envolvidas."*

O objetivo central não é apenas proteger sistemas, mas sim o **ativo "informação"**, independentemente do meio no qual ela está processada, transportada ou armazenada.

---

## Os Atributos Principais (A Tríade CID + Privacidade)

### 1. Confidencialidade
É a propriedade que garante que a informação **não seja disponibilizada ou revelada a indivíduos, entidades ou processos não autorizados**. 
* **Objetivo prático:** Garantir que "só quem pode ver, veja".
* **Mecanismos de controle comuns:** Criptografia de dados (em repouso e em trânsito), Controle de Acesso Baseado em Funções (RBAC) e Autenticação Multifator (MFA).

### 2. Integridade
É a salvaguarda da **exatidão e completude da informação e dos seus métodos de processamento**. Garante que o dado não foi alterado, corrompido ou destruído de maneira não autorizada ou acidental.
* **Objetivo prático:** Garantir que "a informação recebida é estritamente original".
* **Mecanismos de controle comuns:** Funções *Hash* (como SHA-256), assinaturas digitais, controle de versionamento e trilhas de auditoria (*logs*).

### 3. Disponibilidade
É a propriedade de a informação estar **acessível e utilizável sob demanda por uma entidade autorizada**, no momento em que for necessária.
* **Objetivo prático:** Garantir que "o sistema esteja no ar quando o usuário precisar".
* **Mecanismos de controle comuns:** Redundância de servidores (*clusters*), balanceadores de carga, rotinas de *backup* testadas, nobreaks e planos de recuperação de desastres (DRP).

### 4. Privacidade
Diferente da confidencialidade (que foca na proteção de segredos de negócio ou dados internos), a **privacidade refere-se ao direito do indivíduo (titular)** de controlar a coleta, o processamento, o armazenamento, a reutilização e o compartilhamento de seus **dados pessoais**.
* **Objetivo prático:** Respeitar a soberania do usuário sobre suas próprias informações.
* **Base regimental:** No Brasil, é regida rigorosamente pela **LGPD** (Lei Geral de Proteção de Dados - Lei nº 13.709/2018).

  # 2. Ameaças e Vulnerabilidades

Uma **Ameaça** é um evento potencial capaz de explorar uma fragilidade; a **Vulnerabilidade** é a própria fragilidade (a porta destrancada); e o **Risco** é a probabilidade de a ameaça cruzar com a vulnerabilidade gerando impacto.

---

## Exemplos de Ameaças Digitais

1. **Phishing (Pescaria Digital):** Ameaça que utiliza mensagens fraudulentas (e-mail, SMS, WhatsApp) disfarçadas de instituições confiáveis (bancos, Receita Federal, chefes) para induzir o usuário a entregar credenciais ou executar códigos maliciosos.
2. **Malware (Software Malicioso):** Termo genérico para códigos programados para causar dano, roubo ou subversão. Subdivide-se em:
   * **Ransomware:** Criptografa os arquivos do sistema e exige resgate financeiro (geralmente em criptomoedas) pela chave de descriptografia.
   * **Spyware:** Monitora e espia as atividades do teclado ou tela da vítima de forma oculta.
   * **Trojans (Cavalo de Tróia):** Aplicativo aparentemente legítimo que executa funções danosas em segundo plano.
3. **Engenharia Social:**
   Técnica de manipulação psicológica baseada na exploração de vieses cognitivos humanos (urgência, medo, ganância, autoridade, solidez ou vaidade) para burlar barreiras físicas ou lógicas de segurança.

---

## Vulnerabilidades: Técnicas vs. Humanas

| Vulnerabilidades Técnicas | Vulnerabilidades Humanas |
| :--- | :--- |
| • Softwares desatualizados (sem aplicação de *patches*). | • Uso de senhas fracas ou reutilizadas em múltiplos sites. |
| • Portas de rede expostas à internet sem firewall. | • Ausência de malícia/treinamento ao clicar em links externos. |
| • Algoritmos de criptografia obsoletos (ex: WEP em Wi-Fi). | • Anotação de credenciais em locais físicos acessíveis (post-its). |
| • Falhas de lógica em códigos de aplicações corporativas (*SQL Injection*). | • Violação de normas por "pressão de entrega" ou excesso de confiança. |

---

## Impactos Potenciais em Sistemas e Organizações

* **Impactos Financeiros:** Pagamento de extorsões, contratação emergencial de consultorias forenses, perda de faturamento por tempo de inatividade (*downtime*) e multas regulatórias severas (como as aplicadas pela ANPD no âmbito da LGPD).
* **Impactos Operacionais:** Paralisia da cadeia de suprimentos, perda irrecuperável de bancos de dados históricos e paralisação de serviços essenciais (como hospitais ou redes de transporte).
* **Impactos Reputacionais:** Erosão imediata do valor de marca, perda da confiança de clientes e investidores, e evasão de contratos comerciais.
* **Impactos Jurídicos:** Processos judiciais movidos por clientes cujos dados vazaram e responsabilização civil/criminal dos gestores.

  # 3. Estudo de Cenário — Opção A: Ataque Cibernético Real

## O Ataque de Ransomware "WannaCry" (Maio de 2017)

### 1. Contexto do Ataque
Iniciado no dia 12 de maio de 2017, o **WannaCry** (ou *WannaCrypt*) foi um ataque cibernético global de proporções históricas. Em poucas horas, o *malware* infectou mais de **200.000 computadores em 150 países**. 

Entre os alvos de alto perfil atingidos estavam a **Telefónica** (Espanha), a **FedEx** (EUA), a **Petrobras** (Brasil) e, de forma mais dramática, o **NHS** (*National Health Service* - Serviço Nacional de Saúde do Reino Unido). O ataque não exigia que o usuário baixasse um arquivo; uma vez dentro de uma rede corporativa, o software propagava-se autonomamente entre máquinas vizinhas.

### 2. Vulnerabilidade Explorada
O WannaCry explorou uma vulnerabilidade técnica crítica no protocolo de compartilhamento de arquivos **SMBv1** (*Server Message Block*) do sistema operacional Microsoft Windows. 

A ferramenta utilizada para explorar essa falha chamava-se **EternalBlue** — um *exploit* cibernético supostamente desenvolvido pela Agência de Segurança Nacional dos EUA (NSA), que havia sido roubado e vazado publicamente na internet meses antes pelo grupo hacker *The Shadow Brokers*. Embora a Microsoft tivesse liberado uma atualização de segurança para corrigir a falha em março de 2017 (Boletim **MS17-010**), centenas de milhares de organizações negligenciaram a atualização de seus parques tecnológicos.

### 3. Impactos Causados
* **Violação da Tríade CIA:** A **Disponibilidade** foi totalmente destruída nos terminais afetados, e a **Integridade** dos arquivos foi perdida via criptografia de alta complexidade.
* **Caos na Saúde Pública:** No Reino Unido, o NHS precisou cancelar milhares de cirurgias programadas, exames de pacientes oncológicos foram adiados e ambulâncias transportando pacientes de emergência precisaram ser desviadas de hospitais com sistemas paralisados.
* **Prejuízo Econômico:** Estima-se que as perdas globais diretas e indiretas causadas pela paralisação logística e de serviços tenham ultrapassado a marca de **4 bilhões de dólares**.

### 4. Medidas de Mitigação Aplicadas e Recomendadas

#### Medidas de Contingência Imediata (Durante o ataque):
1. **Ativação do *Kill Switch*:** O pesquisador de segurança britânico Marcus Hutchins descobriu que o código do malware tentava se conectar a um domínio não registrado na internet antes de iniciar a criptografia. Ao registrar o domínio por US$ 10, Hutchins ativou o "freio de emergência" global do código, paralisando novas infecções.
2. **Isolamento de Camada:** Organizações desconectaram fisicamente cabos de rede de máquinas Windows antigas e desativaram temporariamente as portas `445` e `139` nos firewalls de borda.

#### Medidas Definitivas de Engenharia de Segurança:
1. **Gestão de Patches (Patch Management):** Estabelecimento de políticas rigorosas e automatizadas de atualização de sistemas operacionais críticos com prazos máximos de homologação.
2. **Desativação de Protocolos Legado:** Abolição definitiva do protocolo *SMBv1* nas redes internas corporativas.
3. **Adoção da Regra de Backup 3-2-1:** * Manter **3** cópias dos dados;
   * Em **2** mídias de tipos diferentes;
   * Com **1** das cópias totalmente *offline* (imune a malwares que varrem a rede).
4. **Segmentação de Rede:** Criação de VLANs estanques para impedir que a contaminação de um terminal de secretaria alcance, por exemplo, o servidor central de um hospital.


### Proposta de Texto para a "Reflexão Individual"

Título: O Fator Humano: Por que a mente é a única vulnerabilidade que não aceita patch?

Na arquitetura de sistemas da informação modernos, investem-se anualmente bilhões de dólares na aquisição de firewalls de próxima geração (NGFW), algoritmos de criptografia assimétrica de padrão militar e softwares de detecção comportamental baseados em Inteligência Artificial. Contudo, a história dos maiores desastres cibernéticos corrobora um axioma cruel: a barreira tecnológica mais avançada do mundo pode ser completamente anulada por um único clique dado no momento errado. O ser humano permanece como o elo mais frágil da corrente de segurança porque computadores operam sob a rigidez da lógica binária, enquanto pessoas operam sob a subjetividade das emoções, dos hábitos e do cansaço.

O primeiro grande motivador dessa fragilidade reside na exploração de vieses cognitivos. A Engenharia Social não ataca sistemas operacionais; ela ataca a psique. Quando um criminoso simula um e-mail urgente da diretoria exigindo uma transferência financeira imediata, ele aciona o gatilho da autoridade e do medo de repreensão. Quando dispara uma mensagem prometendo um prêmio fácil, aciona a ganância. A mente humana evoluiu para buscar cooperação, reciprocidade e atalhos de decisão para economizar energia mental. O atacante cibernético mapeia exatamente esses atalhos evolutivos para transformar a própria vítima em um vetor de invasão interna.

O segundo fator determinante é o fenômeno estudado pela psicologia comportamental como Security Fatigue (Fadiga de Segurança). Medidas de segurança rígidas quase sempre se opõem à usabilidade. Quando uma organização impõe trocas de senhas complexas a cada 30 dias, proíbe o uso de USBs e exige três etapas de verificação para abrir uma simples planilha, o colaborador não se torna mais seguro; ele se torna exausto. Para contornar a fricção cognitiva, ele passa a anotar a senha no verso do teclado, reenvia arquivos corporativos sigilosos para o seu e-mail pessoal do Gmail por ser "mais rápido" e clica em "Aceitar" em avisos de certificados inválidos apenas para conseguir fechar sua demanda do dia.

Por fim, caímos no erro histórico de tratar a cibersegurança exclusivamente como um problema de TI, e não como um problema de cultura. Máquinas são consertadas via atualização de software (patching); seres humanos não recebem atualizações instantâneas de conscientização. A superação dessa fragilidade não será alcançada punindo o usuário que clica no link nocivo, mas sim reconfigurando a engenharia corporativa: implementando arquiteturas Zero Trust (onde o erro humano tem seu raio de explosão minimizado por padrão) e convertendo o colaborador, através de campanhas contínuas e empáticas de Security Awareness, de "elo mais fraco" para a primeira linha de detecção ativa da organização.
