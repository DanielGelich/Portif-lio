# Portif-lio

1. Descrição Do Projeto
   
Tema do projeto
  O projeto envolve a criação de uma plantadeira inteligente que utiliza tecnologia de ponta
para facilitar o cuidado das plantas. O vaso combina sensores de umidade do solo, temperatura e
umidade do ar para monitorar instantaneamente a condição de suas plantas. Os dados são transferidos
para um aplicativo móvel ou web via Wi-Fi, permitindo aos usuários monitorar e gerenciar suas
fábricas remotamente. O sistema também envia mensagens sobre condições em que a planta se
encontra, facilitando para que o usuário consiga cuidar da planta adequadamente. O projeto combina
eletrônica, programação e automação para fornecer uma solução moderna e eficiente que melhora a
experiência de jardinagem para usuários de todos os níveis.

Problemas a Resolver
  ● Monitoramento Ineficiente das Condições do Solo:
  Muitos jardineiros, especialmente iniciantes, têm dificuldade em monitorar a umidade
  do solo de forma precisa, o que pode levar à rega insuficiente ou excessiva das
  plantas.
  
  ● Falta de Dados em Tempo Real:
  A ausência de informações em tempo real sobre as condições ambientais ao redor das
  plantas dificulta a manutenção ideal, resultando em condições de crescimento
  subótimas.
  
  ● Dificuldade em Manter a Saúde das Plantas em Rotinas Ocupadas:
  Pessoas com agendas ocupadas muitas vezes esquecem de regar suas plantas ou não
  estão presentes para atender às suas necessidades, levando ao estresse ou morte das
  plantas.
  
  ● Ausência de Notificações e Alertas Preventivos:
  Sem alertas proativos, os cuidadores de plantas não são informados sobre condições
  adversas, como solo seco, até que seja tarde demais para intervir efetivamente.

Limitações
  ● Nutrientes e Fertilização:
  O projeto não incluirá sensores ou sistemas para monitorar e administrar os níveis de
  nutrientes e fertilizantes no solo. A fertilização adequada continuará sendo responsabilidade
  do usuário.
  
  ● Pestes e Doenças:
  O sistema não terá a capacidade de detectar ou tratar pragas e doenças das plantas. O manejo
  de pragas e doenças requer observação manual e intervenções específicas que o projeto não
  contempla.
  
  ● Luz Solar:
  Embora o vaso monitore a temperatura e a umidade do ar, ele não avaliará a quantidade de luz
  solar recebida pela planta. A posição e a exposição à luz solar devem ser gerenciadas
  manualmente pelo usuário.
  
  ● Condicionamento do Solo:
  O projeto não abordará a qualidade ou a composição inicial do solo, como a textura, o pH ou
  a presença de matéria orgânica. A preparação adequada do solo é uma tarefa inicial que deve
  ser realizada pelo usuário.
  
  ● Variedade de Plantas:
  O sistema pode não ser ajustável para as necessidades específicas de diferentes tipos de
  plantas que requerem condições de crescimento muito específicas. A configuração padrão do
  vaso é destinada a plantas comuns de interior.
  
  ● Conectividade Offline:
  O vaso depende de uma conexão Wi-Fi para enviar dados ao aplicativo. Em ambientes sem
  acesso à internet, o monitoramento e as notificações em tempo real não estarão disponíveis.
  
  ● Intervenções Manuais:
  A automação será limitada ao monitoramento do solo e ambiente. Outras intervenções
  manuais, como poda, regar, replantio ou ajustes na exposição ao ar, não serão automatizadas
  pelo sistema

2. Especificação Técnica
O projeto Smart Planter visa criar uma solução tecnológica avançada para facilitar o cuidado
das plantas, principalmente para pessoas com rotina diária agitada ou pouca experiência em
jardinagem. O sistema consistirá em vários componentes integrados de hardware e software,
proporcionando monitoramento, automação e conectividade em tempo real.

Componentes e Requisitos de Hardware:
  ● Microcontrolador: ESP8266 ou ESP32 para processamento de dados e
  conectividade Wi-Fi.
  ● Sensores: Sensor de Umidade do Solo: Para medir a umidade do solo de forma
  precisa.
  ● Sensor de Temperatura e Umidade do Ar: DHT11 ou DHT22 para monitorar as
  condições ambientais.
  ● Sistema de Irrigação: Bomba de água controlada pelo microcontrolador para
  automação da irrigação.
  ● Fonte de Energia: Baterias recarregáveis ou adaptador AC.
  ● Conectividade: Módulo Wi-Fi integrado (no ESP8266/ESP32).

Requisitos de Software:
  ● Firmware do Microcontrolador:
      1. Desenvolvido na plataforma Arduino IDE.
      2. Leitura e processamento dos dados dos sensores.
      3. Comunicação com o aplicativo móvel ou web via Wi-Fi.
  ● Aplicativo Móvel ou Web:
      1. Arduino Iot Cloud Remote será utilizado para fazer a configuração e
      monitoramento dos dados captados pelos sensores.
      2. Poderá ser feito a conexão web através de uma biblioteca ou o próprio ip que
      a placa arduino irá gerar.
      3. Protocolos de Comunicação:
        ● Wi-Fi: Utilizado para conectar o microcontrolador ao roteador local e enviar dados
        ao aplicativo.     
        ● HTTP/HTTPS: Para comunicação segura entre o microcontrolador e o aplicativo
        móvel ou web.

Algoritmos e Procedimentos:
  ● Leitura dos Sensores:
    1. Procedimento para ler a umidade do solo em intervalos regulares.
    2. Procedimento para ler a temperatura e a umidade do ar.
    
  ● Processamento de Dados:
    1. Algoritmo para determinar quando acionar a irrigação com base na umidade
    do solo.
    2. Algoritmo para enviar dados ao aplicativo e gerar notificações quando os
    níveis críticos são atingidos.
    
  ● Interface do Usuário:
    1. Algoritmo para atualizar a interface do aplicativo com dados em tempo real.
    2. Mecanismo de envio de notificações para alertar o usuário.
    3. Procedimentos de Configuração e Operação:
  ● Configuração Inicial:
    1. Conexão do microcontrolador à rede Wi-Fi.
    2. Instalação e configuração do aplicativo móvel ou web.
    3. Calibração inicial dos sensores.
  ● Operação Diária:
    1. Monitoramento contínuo dos sensores.
    2. Envio de dados ao aplicativo a intervalos regulares.
    3. Recebimento de notificações e alertas no aplicativo.
  ● Manutenção:
    1. Troca de baterias ou recarga (se aplicável).
    2. Verificação e limpeza dos sensores e sistema de irrigação.

3. Requisitos de Software

  Lista de Requisitos
  
  Requisitos Funcionais (RF)
    ● Monitoramento de Umidade do Solo:
    O sistema deve incluir um sensor de umidade do solo que fornece leituras precisas e
    frequentes.
    ● Monitoramento de Temperatura e Umidade do Ar:
    O sistema deve incluir sensores para medir a temperatura e a umidade do ar dentro do
    vaso.
    ● Transmissão de Dados:
    O microcontrolador deve enviar os dados coletados pelos sensores para um aplicativo
    via Wi-Fi.
    ● Visualização em Tempo Real:
    O aplicativo deve exibir os dados em tempo real sobre a umidade do solo,
    temperatura e umidade do ar.
    ● Notificações e Alertas:
    O sistema deve enviar notificações ao aplicativo ou dispositivo quando os níveis de
    umidade do solo estiverem fora dos parâmetros estabelecidos.
    ● Automação da Irrigação:
    O sistema deve acionar automaticamente uma bomba de água para irrigação quando a
    umidade do solo estiver abaixo de um nível crítico configurado.
    ● Armazenamento de Dados Históricos:
    O sistema deve armazenar os dados históricos das leituras dos sensores para análise
    futura e visualização de tendências.
  
  Requisitos Não-Funcionais (RNF)
    ● Facilidade de Instalação e Configuração:
    O sistema deve ser fácil de instalar e configurar pelo usuário final, sem a necessidade
    de conhecimentos técnicos avançados.
    ● Eficiência Energética:
    O sistema deve operar de forma controlada em termos de energia, preferencialmente
    com opções de alimentação por baterias recarregáveis ou painéis solares.
    ● Segurança da Comunicação:
    A comunicação entre o microcontrolador e o aplicativo deve ser segura, utilizando
    protocolos como HTTPS ou MQTT com TLS.
    ● Robustez e Confiabilidade:
    O sistema deve ser robusto e funcionar de maneira confiável em diferentes condições
    ambientais, resistindo à exposição prolongada à umidade e variações de temperatura.
    ● Usabilidade do Aplicativo:
    O aplicativo deve ser intuitivo e fácil de usar, proporcionando uma boa experiência ao
    usuário.
    ● Tempo de Resposta:
    O sistema deve ter um tempo de resposta rápido, atualizando os dados em tempo real
    ou com mínimo atraso.
    ● Durabilidade dos Componentes:
    Os componentes de hardware devem ser duráveis e resistentes a condições úmidas e
    variáveis.
    ● Escalabilidade:
    O sistema deve ser escalável, permitindo a adição de mais sensores ou
    funcionalidades no futuro sem grandes modificações.
    ● Eficiência no Armazenamento de Dados:
    O armazenamento dos dados históricos deve ser controlável, utilizando uma base de
    dados leve e de rápido acesso, como Firebase Database.
    ● Custo Acessível:
    O sistema deve ter um custo acessível para o consumidor final, balanceando
    funcionalidade e preço.

Representação dos Requisitos
![image](https://github.com/user-attachments/assets/ea001c0b-e7a7-4cf0-877c-32190dddb9ad)


Padrões de Arquitetura
  Arquitetura em Camadas (Layered Architecture):
    Descrição: A arquitetura em camadas separa o sistema em diferentes camadas, cada
    uma com responsabilidades distintas. Este padrão facilita a manutenção e a
    escalabilidade do sistema.
    
  Aplicação no Projeto:
    ● Camada de Hardware: Inclui os sensores, microcontrolador, bomba de água
    e fonte de energia.
    ● Camada de Controle: O firmware do microcontrolador que processa os
    dados dos sensores, controla a bomba e gerencia a comunicação.
    ● Camada de Comunicação: O módulo Wi-Fi facilita a troca de dados entre o
    microcontrolador e o aplicativo.
    ● Camada de Apresentação: O aplicativo que apresenta os dados aos usuários
    e recebe as configurações.
    ● Camada de Armazenamento e Backend: Servidor que armazena dados
    históricos e utiliza para poder fazer cálculos de previsão.
    
  Padrão MVC (Model-View-Controller):
    Descrição: O padrão MVC divide a aplicação em três componentes principais: Model
    (dados), View (interface do usuário) e Controller (lógica de controle). Este padrão é
    amplamente utilizado no desenvolvimento de aplicativos móveis e web.
  
  Aplicação no Projeto:
      ● Model: Representa os dados coletados dos sensores (umidade do solo,
      temperatura e umidade do ar) e os dados armazenados no servidor.
      ● View: A interface do aplicativo que exibe os dados em tempo real, gráficos
      históricos.
      ● Controller: A lógica no aplicativo que processa os dados recebidos e lida
      com interações do usuário.
      
  Padrão Observer (Observador):
    Descrição: O padrão Observer define uma dependência um-para-muitos entre
    objetos, permitindo que quando um objeto muda de estado, todos os seus
    dependentes sejam notificados e atualizados automaticamente.
    2. Aplicação no Projeto:
    ● O aplicativo observa as mudanças nos dados enviados pelo
    microcontrolador. Quando o microcontrolador envia novas leituras
    dos sensores, o aplicativo é notificado e atualiza a interface do
    usuário em tempo real.
    
  Padrão Singleton:
    1. Descrição: O padrão Singleton garante que uma classe tenha apenas uma
    instância e fornece um ponto de acesso global a essa instância.
    2. Aplicação no Projeto:
    ● Utilizado no microcontrolador para gerenciar a comunicação Wi-Fi e
    a conexão com o servidor, assegurando que apenas uma instância de
    conexão seja ativa a qualquer momento.
    
  Padrão State (Estado):
  
  Descrição: O padrão State permite que um objeto altere seu comportamento
    quando seu estado interno muda. O objeto parecerá mudar de classe.
    
  Aplicação no Projeto:
    No firmware do microcontrolador, diferentes estados podem ser
    definidos para a operação da bomba de água (por exemplo, idle,
    irrigating, error) e para a conexão Wi-Fi (conectado, desconectado,
    tentando reconectar).
    
  Padrão RESTful:
    Descrição: RESTful é um padrão de arquitetura para criar serviços web
      utilizando métodos HTTP. Este padrão é simples e escalável, ideal para
      comunicações entre sistemas.      
    Aplicação no Projeto:
      A comunicação entre o microcontrolador, aplicativo e o servidor
      segue o padrão RESTful, utilizando métodos HTTP como GET e
      POST para trocar dados.

Modelo C4

![image](https://github.com/user-attachments/assets/389a20ae-542c-43bf-97cf-127ef429177e)

Frameworks e Bibliotecas
  ● Arduino IDE / ESP-IDF (Espressif IoT Development Framework)
    Justificativa:
      1. Arduino IDE: Fornece um ambiente de desenvolvimento simplificado e uma
      vasta coleção de bibliotecas para trabalhar com ESP8266/ESP32, facilitando
      o desenvolvimento de firmware.
      2. ESP-IDF: O framework oficial da Espressif oferece recursos avançados e
      suporte para desenvolvimento com ESP8266/ESP32, incluindo suporte para
      FreeRTOS, que é ideal para projetos mais complexos.
  ● Adafruit Unified Sensor Library
    Justificativa:
      1. Integração com Sensores: Facilita a integração de vários sensores usados no
      projeto, como sensores de umidade do solo e sensores de
      temperatura/umidade do ar, com o microcontrolador.
  ● PubSubClient
  
  ● Justificativa:
    MQTT Client: Implementa o protocolo MQTT para comunicação leve e
    eficiente entre o microcontrolador e o servidor/aplicativo, ideal para
    aplicações IoT.
    
  ● MongoDB/Firebase Realtime Database
    Justificativa:
      1. NoSQL Database: MongoDB e Firebase oferecem armazenamento flexível e
      escalável de dados semiestruturados, ideal para os dados variados e em tempo
      real gerados pelos sensores do vaso inteligente.
  ● Python
    Justificativa:
      1. Scripts e Análise de Dados: Utilizado para criar scripts de automação e
      realizar análise de dados, com suporte a bibliotecas poderosas como Pandas e
      NumPy.
  ● Flask
    Justificativa:
      1. Microframework Web para Python: Facilita a criação de APIs simples
      para integração com o sistema, especialmente útil para tarefas de análise de
      dados e automação.

Ferramentas de Gestão de Projeto
  ● Trello
    1. Descrição: Ferramenta de gerenciamento de projetos baseada em Kanban.
    2. Uso: Planejamento, acompanhamento de tarefas e gestão de equipe.
  ● Google Drive / Dropbox
    1. Descrição: Serviços de armazenamento e compartilhamento de arquivos na nuvem.
    2. Uso: Armazenamento e compartilhamento de documentos e recursos do projeto.

Stack Tecnológica
  ● Firmware do Microcontrolador
    1. Microcontrolador: ESP8266/ESP32
    2. Linguagem: C/C++
    3. IDE: Arduino IDE / PlatformIO
    4. Comunicação: MQTT via PubSubClient

  ● Scripts e Automação
    1. Linguagem: Python
    2. Framework: Flask (para APIs simples)
    3. Bibliotecas: Pandas, NumPy





