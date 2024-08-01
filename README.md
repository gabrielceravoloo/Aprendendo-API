<div align="center">
  <img src="https://github.com/user-attachments/assets/687f794b-2f8f-477b-a8f9-dd31288c6328" alt="Capa do Repositório">
</div>

<h1 align="center"> Exemplos Práticos sobre oque é uma API </h1>

### O que é uma API?

APIs, ou Interfaces de Programação de Aplicações, são tecnologia que permitem que diferentes sistemas e aplicações se comuniquem e compartilhem dados de forma eficiente

<hr>

### Porque usar uma API?

Para você enteder melhor sobre o assunto, vou citar dois exemplos que me ajudaram a entender melhor o conceito de API e como ela realmente pode ser útil na prática

 - **Exemplo 1: Calcular o Frete em uma Loja Online**

> Imagine que você está navegando em uma loja online, como a Sam's Club, e encontra um produto interessante. Antes de finalizar a compra, você precisa saber quanto custará o frete até sua casa. Para isso, você informa seu > CEP e clica no botão para calcular o frete. E se eu te dissesse que essa simples ação de informar seu CEP e verificar o valor está relacionada ao uso de uma API?

Seria inviável para a loja manter um banco de dados com todos os endereços e CEPs do Brasil e criar uma lógica complexa para calcular o frete. As APIs oferecem um serviço terceirizado eficiente que realiza essas tarefas, permitindo que a loja se concentre em outras áreas do negócio

 - **Exemplo 2: Criando um Serviço de Streaming**

> Vamos supor que você queira criar sua própria plataforma de streaming, como a Netflix, por exemplo. Além de desenvolver a plataforma, você precisaria coletar informações sobre um milhão de filmes e séries, como capas, sinopses, notas, informações dos atores, do diretor e muito mais

De onde você tiraria tudo isso? Você realmente vai baixar foto por foto e informação por informação para armazenar no seu banco de dados? Primeiro, isso daria um trabalho gigantesco, e segundo, você passaria mais tempo pesquisando do que programando. Conseguiu entender melhor a situação do problema? É assim que surge a necessidade do uso de APIs

<hr>

### Como funciona um API?

<div align="center">
  <img src="https://github.com/user-attachments/assets/86b1fee0-f251-4f63-9554-fe1956058183" alt="Explicação da API">
</div>

### 1. Sistema A (Cliente):

O Sistema A é responsável por fazer a solicitação, criando uma requisição (request) para obter informações ou serviços, como dados sobre um produto ou informações meteorológicas. Em termos simples, o Sistema A pergunta algo à API

### 2. API:

A API atua como uma ponte entre o Sistema A e o Sistema B, recebendo requisições do Sistema A e encaminhando-as para o Sistema B, além de receber as respostas do Sistema B e enviá-las de volta ao Sistema A. Em resumo, a API facilita a comunicação entre o cliente e o servidor

### 3. Sistema B (Servidor):

O Sistema B é o servidor que recebe a solicitação da API, processa o pedido, busca as informações necessárias e cria uma resposta, que é então enviada de volta para a API e transmitida ao Sistema A. Portanto, o Sistema B responde à pergunta feita pelo Sistema A através da API

<hr>

### Quais são os tipos de API?

<div align="center">
  <img src="https://github.com/user-attachments/assets/e4b755f1-0db7-42c7-b888-bfed5b4787e0" alt="Tipos de API">
</div>

**1. SOAP (Simple Object Access Protocol):**
Um protocolo baseado em XML que opera via HTTP e SMTP. Ele é robusto, fornece padrões rigorosos e inclui extensões de segurança
  - **Pros:** Seguro, extensível, com suporte a transações ACID
  - **Contras:** Pesado, verboso e complexo

**2. REST (Representational State Transfer):** 
Um estilo de arquitetura que usa padrões web existentes, incluindo HTTP. Ele se baseia em métodos padrão (GET, POST, PUT, DELETE) e status codes
  - **Pros:** Simples, escalável, fácil de integrar e usar
  - **Contras:** Não tem um padrão rigoroso; as implementações podem variar

**3. GraphQL:** 
Uma linguagem de consulta para sua API. Ela permite que os clientes solicitem apenas os dados de que precisam
  - **Pros:** Flexível, evita sobrecarga e subutilização de dados, otimizado para dispositivos móveis
  - **Contras:** Curva de aprendizado mais íngreme, complexidade na implementação

**4. gRPC:** 
Baseado em HTTP/2 e desenvolvido pelo Google, utiliza Protocol Buffers como linguagem de interface
  - **Pros:** Rápido, suporte para streaming bidirecional, agnóstico a linguagem
  - **Contras:** Menos amigável para navegadores e redes restritivas

**5. WebSocket:**
Permite comunicação bidirecional entre cliente e servidor. Útil para aplicações em tempo real
  - **Pros:** Real-time, eficiente para uso de dados
  - **Contras:** Complexidade na configuração e gerenciamento de conexões

**6. Webhook:**
Um método para um app enviar informações em tempo real para outro app assim que um evento ocorre
  - **Pros:** Real-time, impulsionado por eventos, reduz pesquisas constantes
  - **Contras:** Segurança, gerenciamento de grandes volumes de eventos

**7. MQTT (Message Queuing Telemetry Transport):**
Um protocolo de mensagens leve, útil para dispositivos de baixa potência em redes potencialmente instáveis
  - **Pros:** Leve, ideal para IoT, eficiente em redes de baixa largura de banda
  - **Contras:** Menos recursos de segurança nativos

**8. AMQP (Advanced Message Queuing Protocol):**
Um protocolo de mensagens focado em mensagens intermediadas por broker
  - **Pros:** Flexível, confiável, orientado a mensagens
  - **Contras:** Mais complexo, maior sobrecarga devido à flexibilidade

> **Observação:**
Não existe um tamanho único para todos quando se trata de estilos de arquitetura de API. O melhor método depende do problema específico que você está tentando resolver, do ambiente em que está operando e dos requisitos do seu sistema. Cada estilo tem seus pontos fortes, e a chave é entender suas necessidades e escolher o melhor ajuste
