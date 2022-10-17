# Projeto Adaptador NES para Geniecom DB9 (aka D-sub-9 ou DE9)

## Objetivo

O objetivo desse projeto é recuperar a memória deste simpático Famiclone e documentar a pinagem do joystick deste Clone do NES que foi vendido no Brasil na década de 90. 
Saiba um pouco mais da história dele [nesse site](https://bojoga.com.br/acervo/consoles-de-mesa/geracao-3/geniecom/).

## Motivação

Tenho um NES Americano onde uso no mesmo um adaptador 8bitdo também chamado de [Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/). 
Este adaptador me permite jogar com qualquer controle bluetooth em meu NES. Particularmente, uso este [controle da 8bitdo](https://www.8bitdo.com/pro2/#Transparent) que, na minha opinião, é um dos melhores que já joguei.

Meu primeiro Nintendo 8 bits foi o Geniecom e por conta dessa saudade e nostalgia, resolvi procurar um para comprar e o achei no [eBay](https://www.ebay.com/itm/134259354667).
O vendedor tem um estoque antigo, talvez de uma loja falida, onde está vendendo não somente o Geniecom mas como também outros produtos da década de 90 que hoje não tem valor financeiro.

O Geniecom foi um Clone fabricado em Tawain, exportado para o Brasil e no Brasil o mesmo era representado pela NTD Eletrônica. Alguma empresa espanhola achou uma boa ideia importar esse vídeogame "brasileiro" e assim o mesmo foi parar na Espanha. E agora, estou eu importando o mesmo da Espanha para o Canadá onde moro... Ou seja, o caminho dele foi Tawain -> Brasil -> Espanha -> Canadá

## Adptador DB-9/DE-9 para NES

O objetivo é usar o 8bitdo Retro Receiver no meu Geniecom, permitindo-me assim jogar com meu controle sem fio no Geniecom assim como faço com o NES.
Para isto, precisa ser criado um adaptador que faça o conector DB9/E9 receber o conector proprietário do NES.

Andando pelo youtube, achei esse vídeo:

[![Sensacional!](https://img.youtube.com/vi/fYj5p7F7-cc/hqdefault.jpg)](https://youtu.be/fYj5p7F7-cc)


Fiquei maravilhado! Esse vídeo me levou para o Shopee onde achei [o gênio por traz do mesmo](https://shopee.com.br/Controle-Nes-8-Bits-Adapter-Para-Jogar-No-Turbo-Game-Phamtom-i.303516671.12405585571?xptdk=4372ea12-6468-4091-833f-f64e535032ac).

Se você tiver um Phantom System, Top Game ou Turbo Game, ele já tem os projetos prontos para venda. [Confere lá](https://shopee.com.br/Controle-Nes-8-Bits-Adapter-Para-Jogar-No-Turbo-Game-Phamtom-i.303516671.12405585571?xptdk=4372ea12-6468-4091-833f-f64e535032ac)

Entrei em contato com ele, que disse que se eu conseguisse o mapa de pinagem do Geniecom, ele poderia fazer o adaptador sem nenhum problema, visto que o projeto seria alterado apenas na ordem dos fios a serem soldados.

### Coleta de Informações

* O NES usa o seguinte [conector com 7 pinos](https://www.nesdev.org/wiki/Controller_port_pinout)
* O Geniecom usa o conector DB9/DE9
* Faltaria-me o mapa de pinagem do Geniecom

## Busca

Procurei pelo Twitter, Reddit, Facebook (posts e grupos), além de Mercado Livre e Shopee. Não encontrei a documentação.
Não desisti, contactei os vendedores do Mercado Livre para saber se algum deles poderia me extrair o mapa, até que essa alma caridosa [desse anúncio me ofereceu o mapa](https://produto.mercadolivre.com.br/MLB-2143952783-geniecom-clone-nes-_JM).

O cara foi gente boa demais! [Comprem logo o Geniecom do anúncio dele porque é confiabilíssimo](https://produto.mercadolivre.com.br/MLB-2143952783-geniecom-clone-nes-_JM)!

E finalmente, sem delongas! O tão procurado mapa de pinagem!

![Mapa Pinagem do Geniecom](https://gitlab.aidentu.com.br/robertofelix/publico/-/raw/main/Geniecom%20DB9%20pinout.png)

## Validação

Irei validar o mapa com o fabricante do adaptador para saber se alguma coisa está faltando. Já falei com um amigo que disse que o mapa passado parece suficiente. Agora é torcer para o projeto finalmente se tornar realidade.


