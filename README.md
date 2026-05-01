# Projeto GuitarCIn

## Apresentação
O **GuitarCIn** é um jogo musical interativo construído com microcontroladores e inspirado na dinâmica do célebre "Guitar Hero". 

Este projeto foi desenvolvido pelos estudantes Jefferson Pereira de Oliveira Júnior e Luiz Felipe Pinto Ávila de Barros, no âmbito da disciplina de Introdução à Computação lecionada pelo professor Adriano Lorena, no Centro de Informática da Universidade Federal de Pernambuco (CIn-UFPE). Inicialmente submetido como projeto para a Feira de Ciências, o GuitarCIn também foi exibido posteriormente no *Open Day* do CIn.

## Dinâmica do Jogo
O funcionamento central do software foca-se na geração e receção de sinais rápidos:
* O sistema gera valores aleatórios (de 0 a 4) que correspondem às teclas da guitarra.
* O utilizador deve pressionar o sensor correto e de forma atempada, consoante o que é indicado no jogo.
* Um sinal sonoro é emitido através de um *buzzer* sempre que o sensor regista um toque.
* Se a nota pressionada for a correta, a partida prossegue.
* Caso o utilizador erre a nota ou pressione múltiplos sensores em simultâneo, o jogo é encerrado.
* A pontuação máxima atingida é gravada através de um sistema de recordes (*high score*).
* Há um botão físico dedicado a reiniciar a partida sem que seja necessário recompilar o software no microcontrolador.

## Componentes de Hardware
A montagem física e eletrónica requereu a integração de diversos módulos:
* 1x Placa Arduino Uno
* 4x Sensores de Toque TPP223B (utilizados como as teclas da guitarra)
* 1x Ecrã com comunicação via protocolo I2C
* 1x *Buzzer* para emissão sonora
* 1x Botão de pressão (*push button*) para a função de reinício
* Cabos Jumper e Protoboard
* Estrutura física montada com cartão em forma de guitarra, finalizada com pintura a tinta guache vermelha em alusão às cores do CIn
