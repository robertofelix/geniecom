# Projeto Adaptador NES para Geniecom db9 (D-sub-9 ou de9)

## Objetivo

O objetivo desse projeto é recuperar a memória deste simpático Famiclone e documentar a pinagem do joystick deste Clone do NES que foi vendido no Brasil na década de 90. Saiba um pouco mais da história dele [nesse site](https://bojoga.com.br/acervo/consoles-de-mesa/geracao-3/geniecom/).

## Motivação

Tenho um NES Americano onde uso no mesmo um adaptador 8bitdo também chamado de [Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/). 
Este adaptador me permite jogar com qualquer controle bluetooth em meu NES. Particularmente, uso este [controle da 8bitdo](https://www.8bitdo.com/pro2/#Transparent) que, na minha opinião, é um dos melhores que já joguei.

Meu primeiro Nintendo 8 bits foi o Geniecom e por conta dessa saudade e nostalgia, resolvi procurar um para comprar e o achei no [eBay](https://www.ebay.com/itm/134259354667).
O vendedor tem um estoque antigo, talvez de uma loja falida, onde está vendendo não somente o Geniecom mas como também outros produtos da década de 90 que hoje não tem valor financeiro.

O Geniecom foi um Clone fabricado em Tawain, exportado para o Brasil e no Brasil o mesmo era representado pela NTD Eletrônica. Alguma empresa espanhola achou uma boa ideia importar esse vídeogame "brasileiro" e assim o mesmo foi parar na Espanha. E agora, estou eu importando o mesmo da Espanha para o Canadá onde moro... Ou seja, o caminho dele foi Tawain -> Brasil -> Espanha -> Canadá

## Adptador DB9/DE9 para NES

O objetivo é usar o 8bitdo Retro Receiver no meu Geniecom, permitindo-me assim jogar com meu controle sem fio no Geniecom assim como faço com o NES.
Para isto, precisa ser criado um adaptador que faça o conector DB9/E9 receber o conector proprietário do NES.

Sobre o conector DB9, [você pode ler mais aqui](http://www.nullmodem.com/DB-9.htm)

Andando pelo youtube, achei esse vídeo:

[![Sensacional!](https://img.youtube.com/vi/fYj5p7F7-cc/hqdefault.jpg)](https://youtu.be/fYj5p7F7-cc)

Se você tiver um Phantom System, Top Game, Geniecom ou Turbo Game, o Lucas Guilherme já tem os projetos prontos para venda. [Confere lá](https://shopee.com.br/shop/353762657)

### Coleta de Informações

* O NES usa o seguinte [conector com 7 pinos](https://www.nesdev.org/wiki/Controller_port_pinout)
* O Geniecom usa o conector DB9/DE9
* Faltaria-me o mapa de pinagem do Geniecom

## Busca

Procurei pelo Twitter, Reddit, Facebook (posts e grupos), além de Mercado Livre e Shopee. Não encontrei a documentação. Até que topei com os anúncios do Lucas no Shopee. Vi as reviews dele que me deu confiança, resolvi adquirir um Geniecom no Mercado Livre e mandei entregar na casa dele em Araraquara. Ele abriu o console, fez a documentação e compartilhou comigo. Adquiri 2 adaptadores com ele mas solicitei o pinout e vou tentar fazer um adaptador aqui para fins educacionais.

E finalmente, sem delongas,  p tão procurado mapa de pinagem!P ara os leigos (como eu) Strobe == Latch.
Lucas ainda consegui identificar o pino pelo qual o Geniecom manda o som para o joystick que tem porta P2.

![Mapa Pinagem do Geniecom](https://github.com/robertofelix/geniecom/blob/main/geniecom_pinout.png)

De forma que iremos comparar com a pinagem do NES

![Mapa Pinagem do NES](https://github.com/robertofelix/geniecom/blob/main/nes-pinout.png)
