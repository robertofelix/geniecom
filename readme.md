# Projeto Adaptador NES para Geniecom db9/de9

## Objetivo

O objetivo desse projeto é recuperar a memória deste simpático Famiclone e documentar a pinagem do joystick deste Clone do NES que foi vendido no Brasil na década de 90. Saiba um pouco mais da história dele [nesse site](https://bojoga.com.br/acervo/consoles-de-mesa/geracao-3/geniecom/).

## Motivação

Tenho um NES Americano onde uso no mesmo um adaptador 8bitdo também chamado de [Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/).
Este adaptador me permite jogar com qualquer controle bluetooth em meu NES. Particularmente, eu uso o [SN30 Pro+](https://www.8bitdo.com/sn30-pro-plus/) que, na minha opinião, é um dos melhores que já joguei. Recentemente, saiu a atualização dele que agora se chama [Pro2](https://www.8bitdo.com/pro2/), com mais botões e outras novidades.

Meu primeiro Nintendo 8 bits foi o Geniecom, por conta dessa saudade e nostalgia, resolvi procurar um para comprar e o achei no [eBay através desse vendedor que mora na Espanha](https://www.ebay.com/itm/134358526809?mkcid=16&mkevt=1&mkrid=711-127632-2357-0&ssspo=55HXj8BsSfS&sssrc=2047675&ssuid=DWiQR02CTjm&widget_ver=artemis&media=COPY). O vendedor tem um estoque antigo, que talvez seja de uma loja falida, onde ele está vendendo não somente o Geniecom mas como também outros produtos da década de 90 que hoje não tem valor financeiro.

O Geniecom foi um Clone fabricado em Tawain, exportado para o Brasil, e no Brasil o mesmo era representado pela NTD Eletrônica. Durante minhas pesquisas, descobri que alguma empresa espanhola achou uma boa ideia importar esse vídeogame "brasileiro" e assim o mesmo foi parar na Espanha. E agora, estou eu importando o mesmo da Espanha para o Canadá onde moro... Ou seja, o caminho dele foi Tawain -> Brasil -> Espanha -> Canadá

## Adaptador db9/de9 para NES

O objetivo é usar o 8bitdo [Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/) no meu Geniecom, permitindo-me assim jogar com meu controle sem fio no Geniecom assim como faço com o NES. Para isto, preciso descobrir o mapa de pinagem do Geniecom para fazer o conector db9/de9 receber o conector proprietário do NES.

Sobre o conector db9/de9, [você pode ler mais aqui](http://www.nullmodem.com/DB-9.htm)

Andando pelo youtube, achei esse vídeo:

[![Sensacional!](https://img.youtube.com/vi/fYj5p7F7-cc/hqdefault.jpg)](https://youtu.be/fYj5p7F7-cc)

Se você tiver um Phantom System, Top Game, Geniecom ou Turbo Game, o Lucas Guilherme já tem os projetos prontos para venda. [Confere lá](https://shopee.com.br/shop/353762657)

## Coleta de Informações

* O NES usa o seguinte [conector com 7 pinos](https://www.nesdev.org/wiki/Controller_port_pinout)
* O Geniecom usa o conector db9/de9
* Faltaria-me o mapa de pinagem do Geniecom

## Busca

Procurei pelo Twitter, Reddit, Facebook (posts e grupos), além de Mercado Livre e Shopee. Não encontrei a documentação. Até que topei com os anúncios do Lucas Guilherme no Shopee. Vi as reviews dele como vendedor que me deram confiança no profissional. Resolvi então adquirir um Geniecom no Mercado Livre e mandei entregar na casa dele em Araraquara. Ele abriu o console, fez a documentação da pinagem e compartilhou comigo. Adquiri 2 adaptadores com ele mas solicitei a mapa de pinagem e vou tentar fazer um adaptador aqui em Montreal.

E finalmente, o tão procurado mapa de pinagem! Lucas ainda consegui identificar o pino pelo qual o Geniecom manda o som para o joystick que tem porta P2.

![Mapa Pinagem do Geniecom](https://github.com/robertofelix/geniecom/blob/main/geniecompinout.png)

De forma que iremos comparar com a pinagem do NES

![Mapa Pinagem do NES](https://github.com/robertofelix/geniecom/blob/main/nes-pinout.png)

Para os leigos (como eu) **Strobe == Latch**

## Elaboração do adaptador

Como o Geniecom tem os conectores db9/de9 fêmeas muito profundos, o macho também precisa ser profundo o suficiente para conexão ser perfeita, sem folgas. Resolvi comprar um controle do Mega Drive de 6 botões para reaproveitar o conector dele já que ele tem as dimensões ideais para conectar no Geniecom.

Contudo, é importante notar que precisamos do mapa de pinagem do [Mega Drive 6-Button (X,Y,Z) Controller o qual achei aqui](https://www.raspberryfield.life/2019/03/25/sega-mega-drive-genesis-6-button-xyz-controller/#SMD6-protocol-overview).

![Mapa Pinagem do Mega Drive 6-Button](https://github.com/robertofelix/geniecom/blob/main/genesis.png)

