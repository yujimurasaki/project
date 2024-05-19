<h1>Sensor de Batimentos Cardíacos com Internet das Coisas</h1>
PO projeto visa desenvolver um sensor de batimentos cardíacos utilizando a
plataforma o módulo NodeMCU ESP8266. Através de um sensor de pulso, o
dispositivo é capaz de monitorar os batimentos cardíacos em tempo real.
Posteriormente, o projeto processa essas informações e as apresenta em um
display remoto no qual deve ser conectado pela rede. Essa abordagem oferece
uma solução acessível para o monitoramento cardíaco.


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
<p>https://dl.espressif.com/dl/package_esp32_index.json</p>
<p>Clique em "OK" para salvar.</p>

<h3>Instalação do ESP8266</h3>
<p>• Abra a IDE do Arduino "Files -> Preferences"</p>
<p>• Additional boards manager URL's: http://arduino.esp8266.com/stable/package_esp8266com_index.json</p>
<p>• Tools -> Boards -> Boards Manager... </p>
<p>• Pesquise por esp8266 e instale o pacote </p>


<h3>Instalação das Bibliotecas </h3>
<p>• Sketch -> Include Library -> Manage Libraries... </p>
<p>• Pesquise por PubSubClient para comunicação com protocolo MQTT </p>
<p>• Pesquise por ESP8266WiFi  para comunicação com WiFi </p>

<h3>Configuração para utilização </h3>
<p>Dentro do próprio código foi comentado detalhadamente o que deve ser realizado para funcionar o código </p>


<h2>Conexão via HiveMQ </h2>
<p>É necessário a utilização do site https://www.hivemq.com/demos/websocket-client/ para poder acessar via WiFi </p>
<p>Configure o HIVEMQ da seguinte maneira: </p>
<p> >Host: mqtt.eclipseprojects.io</p>
<p> >Port: 443</p>
<p> >Client: ClientBatimentos</p>
<p> >Connect </p>
<p> >Subscriptions -> Add New Topic Subscription </p>
<p> >Topic: sensor/bpm</p>






<h2> Documentação das interfaces, protocolos e módulos de comunicação utilizados </h2>
<p> ESP8266 TECHNICAL REFERENCES https://www.espressif.com/sites/default/files/documentation/esp8266-technical_reference_en.pdf </p>
<p> WiFi(802.11) https://embarcados.com.br/a-evolucao-do-protocolo-wi-fi-ieee-802-11/ </p>
<p> MQTT https://aws.amazon.com/pt/what-is/mqtt/#:~:text=O%20protocolo%20MQTT%20define%20um,envolvida%20em%20um%20envelope%20WSS </p>
<p>Esp8266Wifi Library https://arduino-esp8266.readthedocs.io/en/latest/esp8266wifi/readme.html </p>
<p>PubSubClient https://www.arduino.cc/reference/en/libraries/pubsubclient/ </p>
