# Fabeacon
Raspberry Pi, Telemóvel ou PC com Boletim Informativo e Plano 333

Saber mais sobre o Boletim: https://macanudos.org/boletim-informativo-na-banda-do-cidadao/
Saber mais sobre o Plano de Comunicações 333: https://macanudos.org/plano-de-emergencia-3-3-3/

O presente código tranforma o dispositivo num emissor. Pode ser instalado em Telemóveis Android; raspberry pi ou qualquer pc.

Fabeacon Author: Rolando Reset

Website: https://github.com/roltel

Fabeacon Code Source: https://github.com/roltel/fabeacon


# Instalação

1. Fazer download do instalador **fabeacon-install.sh**
2. Tornar o instalador executável: 
> chmod 755 fabeacon-install.sh
3. Executar o instalador:
> bash fabeacon-install.sh
4. Após a instalação concluida, todas as configurações necessárias foram realizadas e o Fabeacon é executado automáticamente.

# Desinstalação

1. Executar o instalador:
> bash fabeacon-install.sh
2. Seleccionar a opção de desinstalação.
2. Após a desinstalação concluida, o Fabeacon foi retirado do seu dispositivo.

# Notas Gerais e Suporte
  
Abaixo encontra-se uma versão que usa o Openwebrx (SDR) caso o dispositivo tenha ou venha a ter pen RT8L SDR que só funciona em RPi já preconfigurado com o painel de administração, a vpn e outras ferramentas privadas.

FABEACON "OS": Openwebrx & Fabeacon 
Puxar a seguinte imagem e flashar: 

Conteúdo:
- OS Openwebrx (para se quiser que um dia o sistema tb funcione como sdr)
- Python para usar o GPIO e ligar o pin 17 BCM que é o Board n.º 11
- Jingle Boletim e roger beep 333
- Cron - ficheiro com as rotinas

==VPN== 
A VPN permite que possa controlar o RPI dentro de uma rede privada dando acesso não só ao painel de administraçáo abaixo como também acesso interno ao SDR (caso tenha a pen ligada) ou interligação com outros sistemas.
A VPN instalada acima. Bastará meter o ficheiro fabeaconXX.conf que lhe foi enviado na pasta /etc/openvpn/. Como? Usando o shh scp para copiar de outro sistema ou o filezilla (cliente SFTP); 

Painel de controle:
https://futuragora.pt/futurai/priv/radioadmin

- Emitir Boletim
- Emitir Boletim Digital RTTY
- Emitir Plano 333
- Emitir audio gravado na página.

- Ligar a Portadora
- Desligar a Portadora

Disclaimer: As emissões dos ficheiros audio gerados pelo presente código-livre estão sujeitas às suas condicionantes legais e são da esclusiva responsabilidade das estações que as emitiem.
