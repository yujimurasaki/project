<h1>Sensor de Batimentos Cardíacos com Internet das Coisas</h1>
Projeto criado com Arduino IDE para uma solução simples e alternativa para monitoramento de frequência cardíaca.
<h2>Componentes utilizados para a montagem do protótipo:</h2>
<p> •	1 x ESP8266 NodeMCU; </p>
<p> •	1 x Cabo Micro USB compatível com NodeMCU ESP8266; </p>
<p> •	1 x Sensor de batimento cardíaco / Monitor de pulso; </p>
<p> •	Jumpers macho-fêmea </p>
<p> • Protoboard </p>

<h2>Passo a passo para utilização do projeto </h2>
<h3> Instalação da IDE do Arduino</h3>
<p>Baixar a IDE do Arduino: </p>
<p>Acesse o site oficial do Arduino. Navegue até a seção de downloads e escolha a versão da IDE do Arduino compatível com seu sistema operacional (Windows, macOS ou Linux). Instalar a IDE:</p>
<p>Windows: Execute o instalador baixado e siga as instruções na tela. Certifique-se de instalar todos os drivers necessários durante o processo de instalação. macOS: Abra o arquivo .zip baixado e arraste o aplicativo Arduino para a pasta "Aplicativos". Linux: Descompacte o arquivo baixado e execute o script de instalação. Verificar a Instalação:</p>
<p>Abra a IDE do Arduino para garantir que foi instalada corretamente. Configurando a ESP32 na IDE do Arduino Adicionar o URL do Gerenciador de Placas para a ESP32:</p>
<p>Na IDE do Arduino, vá até "Arquivo" > "Preferências". No campo "URLs Adicionais de Gerenciadores de Placas", insira o seguinte URL para o pacote da ESP32:</p>

<p>É necessário a utilização do site https://www.hivemq.com/demos/websocket-client/ para poder acessar via WiFi </p>

<h2> Documentação das interfaces, protocolos e módulos de comunicação utilizados </h2>
<p> ESP8266 TECHNICAL REFERENCES https://www.espressif.com/sites/default/files/documentation/esp8266-technical_reference_en.pdf </p>
<p> WiFi(802.11) https://embarcados.com.br/a-evolucao-do-protocolo-wi-fi-ieee-802-11/ </p>
<p> MQTT https://aws.amazon.com/pt/what-is/mqtt/#:~:text=O%20protocolo%20MQTT%20define%20um,envolvida%20em%20um%20envelope%20WSS </p>
<p>Esp8266Wifi Library https://arduino-esp8266.readthedocs.io/en/latest/esp8266wifi/readme.html </p>
<p>PubSubClient https://www.arduino.cc/reference/en/libraries/pubsubclient/ </p>
