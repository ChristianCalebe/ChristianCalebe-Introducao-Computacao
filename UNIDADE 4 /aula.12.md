# Aula 12 – Internet: História, Conceitos, Protocolos e Navegadores

## Objetivo
Compreender a origem e evolução da Internet, seus conceitos fundamentais, principais protocolos de comunicação e o papel dos navegadores.

## Estrutura da Entrega
Cada grupo deve incluir neste repositório:

### 1. História da Internet
- Breve resumo da evolução da Internet:
  - ARPANET (década de 60/70).
  - Expansão acadêmica/militar.
  - Comercialização nos anos 90.
  - Criação da WWW por Tim Berners-Lee.

### 2. Conceitos Fundamentais
- Diferenciar **Internet vs. Web**.
- Explicar a **arquitetura cliente-servidor**.
- Exemplificar o uso de endereços **IP**.

### 3. Protocolos
- Analisar os seguintes protocolos:
  - **TCP/IP**
  - **HTTP/HTTPS**
  - **DNS**
  - **FTP**
- Explicar a função de cada protocolo e dar exemplos práticos.

### 4. Navegadores
- Função dos navegadores na interpretação de HTML, CSS e JavaScript.
- Principais motores de renderização:
  - Blink (Chrome/Edge)
  - Gecko (Firefox)
  - WebKit (Safari)

### 5. Exercício Prático – Análise de Protocolos
- Utilizar ferramentas como **Wireshark** ou o **Inspetor do Navegador (F12)**.
- Registrar:
  1. **Request** (requisição feita pelo cliente).
  2. **Response** (resposta do servidor).
  3. **Status Code** (ex.: 200 OK, 404 Not Found).
- Produzir relatório ou slides com os resultados.

## Organização dos Arquivos
- Criar uma pasta com o nome do grupo (ex.: `Grupo1_Protocolos`, `Grupo2_Navegadores`).
- Dentro da pasta, incluir:
  - `historia_internet.pdf` ou `historia_internet.md`
  - `conceitos.pdf` ou `conceitos.md`
  - `protocolos.pdf` ou `protocolos.md`
  - `navegadores.pdf` ou `navegadores.md`
  - `analise_protocolos.pdf` ou `analise_protocolos.png`
  - `README.md` com breve descrição do trabalho.

## Critérios de Avaliação
- Clareza e organização das explicações.
- Correção conceitual na análise dos protocolos.
- Exemplos práticos bem escolhidos.
- Participação de todos os integrantes.

## Reflexão Individual
Cada integrante deve produzir um texto curto (1 página) respondendo:  
**“Qual protocolo você considera mais essencial para o funcionamento da Internet e por quê?”**
Embora a internet seja uma composição interdependente de tecnologias, considero o protocolo IP (Internet Protocol) como o mais essencial para o funcionamento da rede global.
A justificativa reside no fato de que o IP atua na camada de rede, sendo o responsável direto por unificar e dar uma identidade lógica a qualquer dispositivo no planeta. Sem as regras fundamentais de endereçamento e roteamento fornecidas pelo IP (seja na versão IPv4 ou IPv6), seria impossível para os demais protocolos operarem. O HTTP não teria para onde enviar uma página web, o DNS não teria um endereço numérico para mapear e o TCP não saberia para onde destinar seus pacotes de dados.
O IP funciona como a fundação de concreto de um edifício: sem ele, nenhuma das aplicações modernas que utilizamos no dia a dia da Engenharia de Software existiria, tornando-o o verdadeiro pilar da conectividade mundial.
