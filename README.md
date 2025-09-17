# redes2configga
Configuração do trabalho feito no GA, sobre a topologia e protocolos usados.

Trabalho realizado no Software Cisco Packet Tracer
Link Download: https://learningnetwork.cisco.com/s/question/0D53i00000Kt599CAB/download-packet-tracer

Protocolo RIP
Imagem da Topologia usada
![image](https://github.com/user-attachments/assets/d954eb03-9a55-4015-aaa4-6225f3ad3745)
Link para rodar a topologia e configuração feita no Packet Tracer: 
https://drive.google.com/file/d/1C7fRZ1jemweF_rZQZ5d3hFzz4-gYS8JF/view?usp=sharing

Configuração dos IPs dos Roteadores e Computadores

192.168.0.0
PC0 - 192.168.0.2
Router0 - 192.168.0.1

Comando "show ip protocols" mostrando o protocolo RIP em exceução no Route0
![image](https://github.com/user-attachments/assets/395646c6-1586-458b-9300-c5d5f17a26e9)



192.168.1.0
Router0 - 192.168.1.2
Router1 - 192.168.1.1

192.168.2.0
Router1 - 192.168.2.1
Router1 - 192.168.2.2

192.168.3.0
Router2 - 192.168.3.1
PC1 - 192.168.3.3

192.168.4.0
PC2 - 192.168.4.2
Router2 - 192.168.4.1

Taxa de Transmissão
8ms para enviar um pacote de 32 bytes do PC0 para o PC1 e receber a resposta de volta ao PC0, usando protocolo RIP



Protocolo BGP
![image](https://github.com/user-attachments/assets/750aa6f7-12be-4087-b8d2-c16c9bedf60e)
Link para rodar a topologia e configuração feita no Packet Tracer: 
https://drive.google.com/file/d/1eNpBMRJdBMq-BS7mLW3i0NXpxIz-ZogW/view?usp=sharing


Configuração dos IPs dos Roteadores, Computadores e AS

192.168.0.0
PC0 - 192.168.0.2
Router0 - 192.168.0.1
Vizinhos Router0: 192.168.5.2 | 192.168.1.1

Comando "show ip protocols" mostrando o protocolo BGP em exceução no Route0
![image](https://github.com/user-attachments/assets/24e95ee5-c4e7-4769-a1dd-6c06a630f7b9)
AS-180

192.168.2.0
PC1 - 192.168.2.2
Router1 - 192.168.2.1
Vizinhos ROuter1: 192.168.5.3 |  192.168.1.2
AS-171

192.168.4.0
PC2 - 192.168.4.2
Router2 - 192.168.4.1
Vizinhos Router2: 192.168.5.3 | 192.168.3.1
AS-200

192.168.1.0
Router0 - 192.168.1.2
Router1 - 192.168.1.1

192.168.3.0
Router1 - 192.168.3.1
Router2 - 192.168.3.3

192.168.5.0
Router2 - 192.168.5.2
Router0 - 192.168.5.3

Taxa de transmissão
7ms para enviar um pacote de 32 bytes do Router2 para o Router0, usando protocolo BGP

