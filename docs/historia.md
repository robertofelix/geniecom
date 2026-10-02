# A história por trás do projeto

[← Voltar ao README](../README.md)

## Motivação

Tenho um NES americano em que uso o adaptador [8BitDo Retro Receiver](https://www.8bitdo.com/retro-receiver-nes/) para jogar sem fio. Ele permite usar qualquer controle Bluetooth no NES. Eu uso o [SN30 Pro+](https://www.8bitdo.com/sn30-pro-plus/), um dos melhores controles que já usei. Recentemente saiu o sucessor, o [Pro 2](https://www.8bitdo.com/pro2/), com mais botões e outras novidades. Também tenho um e recomendo.

Meu primeiro Nintendo de 8 bits foi o Geniecom. Por saudade e nostalgia, resolvi procurar um para comprar e o achei no [eBay, com um vendedor que mora na Espanha](https://www.ebay.com/itm/134358526809). Ele tem um estoque antigo, que talvez seja de uma loja falida, e vende não só o Geniecom, mas também outros produtos da década de 90.

## O console

O Geniecom é um Famiclone fabricado em Taiwan e exportado para o Brasil, onde era representado pela NTD Eletrônica. Durante as pesquisas, descobri que uma empresa espanhola importou esse videogame "brasileiro" e o vendeu na Espanha com o nome [Mx Onda MX-VJ30S](https://www.va-de-retro.com/foros/viewtopic.php?t=2888). Pelo jeito, também houve unidades vendidas na Espanha com o nome Geniecom. Agora estou importando o console da Espanha para o Canadá, onde moro. O caminho dele foi Taiwan → Brasil → Espanha → Canadá, ou apenas Taiwan → Espanha → Canadá. Quem sabe?

O Geniecom chegou impecável. O único "defeito" é que veio no formato [PAL](https://en.wikipedia.org/wiki/PAL#PAL_region), o que faz sentido, já que veio da Espanha, onde esse era o padrão. Contei com a ajuda do [Ícaro Jonas](https://github.com/icaroj), que trocou a CPU, a PPU e o cristal oscilador por peças do padrão NTSC. Para isso, tive que sacrificar um NES reserva e o tempo do Ícaro :D

## A busca pela pinagem

Procurei no Twitter, no Reddit, no Facebook (posts e grupos), no Mercado Livre e na Shopee. Não encontrei a documentação em lugar nenhum da internet. Ela simplesmente não existia. Até que topei com os anúncios do Lucas Guilherme na Shopee. Vi as avaliações dele como vendedor, que me deram confiança na pessoa e no profissional.

Resolvi então comprar um Geniecom usado no Mercado Livre e mandei entregar na casa dele, em Araraquara. Ele abriu o console, fez pequenos reparos de solda, documentou a pinagem e compartilhou a informação comigo. Comprei um adaptador com o Lucas, mas, com o mapa de pinagem em mãos, resolvi fazer um adaptador aqui em Montreal. Mais uma vez entrou em cena o [Ícaro Jonas](https://github.com/icaroj) que, seguindo a documentação do Lucas, confeccionou dois adaptadores para mim <3

O Lucas também identificou o pino pelo qual o Geniecom envia o som para o joystick. O joystick do Geniecom tem uma saída de áudio P2 (o "banana pequeno", no popular), algo muito à frente do seu tempo. Como o NES não tem essa função, o sinal de som (pino 2 do Geniecom) é ignorado no adaptador.

## Famicom e a porta DB15

O Lucas concluiu que a pinagem da porta DB15 do Geniecom segue o mesmo padrão do Famicom. Ou seja, a [Light Gun](https://www.ebay.com/sch/i.html?_nkw=Gun+light+famicom&_sacat=0) do Famicom funciona no Geniecom, o que foi testado e confirmado.

Com isso em mente, pensei: por que não procurar um adaptador Famicom → NES? Encontrei um na [MisterAddons](https://misteraddons.com/products/nes-controllers-to-famicom-console-adapter), comprei e aguardei a chegada.

Quando o adaptador chegou, consegui conectar dois controles de NES ao Geniecom pela porta DB15. Também consegui ligar a [Zapper](https://en.wikipedia.org/wiki/NES_Zapper) do NES ao conector 2 do adaptador. Nunca vi na internet alguém dizer que ligou uma Zapper, ou qualquer outra pistola, no Geniecom. Também acho que ninguém nunca viu uma pistola sendo vendida para o Geniecom.

## Agradecimentos

Ao [Lucas Guilherme](https://shopee.com.br/shop/353762657), que topou o desafio pelo prazer do conhecimento e da novidade. Não tenho como recomendá-lo mais: foi muito companheiro neste projetinho.

Ao [Ícaro Jonas](https://github.com/icaroj), que converteu o Geniecom para NTSC e fez os cabos usando o mapa fornecido pelo Lucas.

Vocês são 10/10! Também reconheço minha insistência em procurar incessantemente por essa informação, até o ponto de gastar algum dinheiro, mas gerando conteúdo novo para ser compartilhado com os fãs do Geniecom :-)
