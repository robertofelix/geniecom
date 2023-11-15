# Projeto Adaptador NES para Geniecom db9/de9

## Objetivo

O objetivo desse projeto é recuperar a memória deste simpático Famiclone e documentar a pinagem do joystick deste Clone do NES que foi vendido no Brasil na década de 90. Saiba um pouco mais da história dele [nesse site](https://bojoga.com.br/acervo/consoles-de-mesa/geracao-3/geniecom/).

## Motivação

Tenho um NES Americano onde uso no mesmo um adaptador 8bitdo [Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/). Este adaptador me permite jogar com qualquer controle bluetooth no NES. Particularmente, eu uso o [SN30 Pro+](https://www.8bitdo.com/sn30-pro-plus/) que, na minha opinião, é um dos melhores que já usei. Recentemente, saiu a atualização do mesmo que agora se chama [Pro2](https://www.8bitdo.com/pro2/), com mais botões e outras novidades, eu também o tenho e recomendo.

Meu primeiro Nintendo 8 bits foi o Geniecom, por conta dessa saudade e nostalgia, resolvi procurar um para comprar e o achei no [eBay através desse vendedor que mora na Espanha](https://www.ebay.com/itm/134358526809?mkcid=16&mkevt=1&mkrid=711-127632-2357-0&ssspo=55HXj8BsSfS&sssrc=2047675&ssuid=DWiQR02CTjm&widget_ver=artemis&media=COPY). O vendedor tem um estoque antigo, que talvez seja de uma loja falida. O certo é que ele está vendendo não somente o Geniecom mas como também outros produtos da década de 90 que hoje não tem valor financeiro.

O Geniecom foi um Famiclone fabricado em Tawain e exportado para o Brasil, onde no Brasil o mesmo era representado pela NTD Eletrônica. Durante minhas pesquisas, descobri que alguma empresa espanhola achou uma boa ideia importar esse vídeogame "brasileiro" e assim o mesmo foi parar na Espanha sob o nome de [Mx Onda MX-VJ30S](https://www.va-de-retro.com/foros/viewtopic.php?t=2888). Porém, pelo jeito também houve unidades vendidas na Espanha com o nome Geniecom. Agora, estou eu importando o mesmo da Espanha para o Canadá onde moro. Ou seja, o caminho dele foi Tawain -> Brasil -> Espanha -> Canadá, ou apenas Tawain -> Espanha -> Canadá, quem sabe?!

O Geniecom chegou em minha casa impecável. Único 'defeito' era que ele veio transcodificado no formato [PAL](https://en.wikipedia.org/wiki/PAL#PAL_region), o que faz completo sentido já que ele veio da Espanha cujo o padrão era esse. De forma que tive que contar com a ajuda de o [Ícaro Jonas](https://github.com/icaroj) que trocou a CPU, PPU e o Cristal dele, colocando as respectivas peças em padrão NTSC. Para isso, tive que sacrificar um NES reserva e o tempo do Ícaro :D

## Adaptador db9/de9 para NES

O objetivo é usar o 8bitdo [Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/) no Geniecom, permitindo assim jogar com o controle sem fio assim como faço com o NES. Para isso, preciso descobrir o mapa de pinagem do Geniecom para fazer o conector db9/de9 receber o conector proprietário do NES.

Sobre o conector db9/de9, [você pode ler mais aqui](http://www.nullmodem.com/DB-9.htm)

Andando pelo youtube, achei esse vídeo:

[![Sensacional!](https://img.youtube.com/vi/fYj5p7F7-cc/hqdefault.jpg)](https://youtu.be/fYj5p7F7-cc)

Se você tiver um Phantom System, Top Game, Geniecom ou Turbo Game, o Lucas Guilherme já tem os adaptadores prontos para venda. [Confira aqui](https://shopee.com.br/shop/353762657)

## Coleta de Informações

* O NES usa o seguinte [conector com 7 pinos](https://www.nesdev.org/wiki/Controller_port_pinout)
* O Geniecom usa o conector db9/de9
* Falta o mapa de pinagem do Geniecom

## Busca

Procurei pelo Twitter, Reddit, Facebook (posts e grupos), além de Mercado Livre e Shopee. Não encontrei a documentação em canto nenhum na internet, não existia. Até que topei com os anúncios do Lucas Guilherme no Shopee. Vi as reviews dele como vendedor, que me deram confiança na pessoa e no profissional. 

Resolvi então adquirir um Geniecom usado no Mercado Livre e mandei entregar na casa dele em Araraquara. Ele abriu o console, fez pequenos reparos de solda, e fez a documentação da pinagem, compartilhando a informação comigo. Adquiri 01 adaptador com o Lucas mas o solicitei o mapa de pinagem para fazer um adaptador aqui em Montreal. Mais uma vez, entra em cena [Ícaro Jonas](https://github.com/icaroj) que, seguindo a documentação do Lucas, confeccionou dois adaptadores para mim <3

E finalmente, o tão procurado mapa de pinagem! Lucas ainda consegui identificar o pino pelo qual o Geniecom envia o som para o joystick, lembrando que o joystick do Geniecom tem uma porta de áuido P2, coisa muito a frente de seu tempo. Como o NES não tem a mesma função, iremos ignorar o Sound que está mapeado na Port 2 do Geniecom.

### Geniecom Pinout Gamepad Facing

Perspectiva olhando o conector do controle frontalmente.

![Mapa Pinagem do Geniecom Gamepad Facing](https://github.com/robertofelix/geniecom/blob/main/geniecom_gamepad_facing.png)

### Geniecom Pinout Console Facing

Perspectiva olhando o conector do console frontalmente.

![Mapa Pinagem do Geniecom Console Facing](https://github.com/robertofelix/geniecom/blob/main/geniecom_console_facing.png)

### Famicom e Genicom Pinout Console Facing

O Lucas percebeu que a pinagem da porta db15 do Geniecom tinha o mesmo padrão do Famicom. Ou seja, a [Gun Light](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p4432023.m570.l1312&_nkw=Gun+light+famicom&_sacat=0) do Famicom deve funcionar no Geniecom. No futuro, irei comprar uma e testar. 

![Mapa Pinagem do Famicom e Geniecom](https://github.com/robertofelix/geniecom/blob/main/famicom_console_facing.png)

### NES Pinout

De forma que iremos comparar com a pinagem do NES.

![Mapa Pinagem do NES](https://github.com/robertofelix/geniecom/blob/main/nes_pinout.png)

### NES e Famicom comparados

Apenas um extra, comparamos a pinagem do NES e Famicom fazendo a correlação com a porta db15.

![Mapa Pinagem do NES e Famicom comparados](https://github.com/robertofelix/geniecom/blob/main/nes_famicom_pinout.png)

### Terminologia

Para os leigos (como eu):

* Strobe == Latch
* Power == VCC +5V

## Elaboração do adaptador

Como o Geniecom tem os conectores db9/de9 machos muito longos, a fêmea também precisa ser longa o suficiente para conexão ser perfeita, sem folgas. Para fazer o adaptador perfeito, tive que comprar:

* [Cabo Extensor para controle do Mega Drive](https://www.aliexpress.com/item/4000095438635.html?spm=a2g0o.order_list.order_list_main.17.231b1802wecZG5)
* [Cabo Extensor para o controle do NES](https://www.aliexpress.com/item/4000029468234.html?spm=a2g0o.order_list.order_list_main.5.231b1802wecZG5)
* [Ferrite core cord ring 5mm](https://www.aliexpress.com/item/1005006071819843.html?spm=a2g0o.order_list.order_list_main.11.231b1802wecZG5)

Em resumo, foram cortados os cabos do extensor do Mega Drive e do NES. Depois disso, foi feito o mapeamento de cada pino do db9/de9 do Mega Drive.

Mega Drive -> Geniecom

| Port | Color | Function |
| --- | --- | --- |
| 01 | Red | GND (Ground) |
| 02 | Black | Sound |
| 03 | Grey | Latch |
| 04 | Orange | x |
| 05 | Brown | Data |
| 06 | Green | Clock |
| 07 | White | x |
| 08 | Blue | x |
| 09 | Yellow | VCC +5V |

NES
| Port | Color | Function |
| --- | --- | --- |
| 01 | White | GND (Ground) |
| 02 | Green | Clock |
| 03 | Yellow | Latch |
| 04 | Black | Data |
| 05 | Red | VCC +5V |
| 06 | x | x |
| 07 | x | x |

## Resultado Final

Esta belezinha!

![Adaptador Geniecom - NES](https://github.com/robertofelix/geniecom/blob/main/adaptadornesgeniecom.png)

## Bônus

Pinagem dos demais clones que consegui coletar:

![Clone Wars](https://github.com/robertofelix/geniecom/blob/main/demais_clones_pinout.png)

## Agradecimentos

Ao [Lucas Guilherme](https://shopee.com.br/shop/353762657) que topou o desafio pelo prazer do conhecimento e da novidade. Não tenho como recomendar mais o cara, foi muito companheiro nesse projetinho. E ao [Ícaro Jonas](https://github.com/icaroj) que transcodificou o Geniecom assim como fez o cabo usando o mapa fornecido pelo Lucas. Vocês são 10/10! Também reconhecer minha insistência em ficar procurando incessantemente isso, até chegar ao ponto de ter que gastar algum dinheiro porém gerando conteúdo novo para ser compartilhado com os fãs do Geniecom :-)