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
Apesar de a internet ser um ecossistema complexo e interdependente, o protocolo IP (Internet Protocol) destaca-se como o elemento mais vital para a operação da rede global. Sua importância deve-se à sua atuação na camada de rede, onde é o principal responsável por atribuir uma identidade lógica e universal a cada dispositivo. Sem a base estrutural de endereçamento e roteamento do IP (em suas versões IPv4 ou IPv6), a operação dos demais protocolos seria inviável. O HTTP não teria um destino para entregar páginas, o DNS não possuiria IPs numéricos para resolver e o TCP não conseguiria guiar seus pacotes de dados. O IP é, portanto, a fundação estrutural da internet: sem ele, as soluções modernas da Engenharia de Software seriam impossíveis, consagrando-o como o verdadeiro pilar da comunicação digital.
