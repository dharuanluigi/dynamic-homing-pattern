<!-- @format -->

# Dynamic Homing Pattern 🚀 ↩️

![Version](https://img.shields.io/badge/version-1.0-blue)
![Document type](https://img.shields.io/badge/documentation-Chatbot%20Desing%20Pattern-brightgreen)
<a href="http://creativecommons.org/licenses/by-sa/4.0/" target="_blank"><img src="https://img.shields.io/badge/license-Attribution--ShareAlike%204.0%20International-orange" /></a>

## Sobre

Este repositório tem o intuito de mostrar informações mais detalhadas do design pattern que chamei de Dynamic Homing, usado para desenvolver chatbots que usam plataformas orientadas a microserviços. Criei esse Pattern com o intuito e preocupação na padronização e qualidade de desenvolvimento de chatbots que utilizam Blip. Neste contexto, o uso e distribuição é totalmente aberto e para a comunidade, alterações e modificações são muito bem-vindas, desde que sigam e mentenham a mesma licença de uso.

<div style="display: flex;">
   <span style="margin: 0 auto;">Criado por mim com muito 💜.</span>
</div>

## O que é?

Caso você tenha chego aqui e ainda não leu [meu artigo do Medium](https://medium.com/@dharuanluigi/dynamic-homing-pattern-o-design-pattern-para-chatbot-introdu%C3%A7%C3%A3o-420a3f48fdb9), onde eu apresento detalhes sobre esse Pattern, sugiro que tire um tempinho antes de seguir lendo e consumindo diretamente deste repositório. Mas caso queira continuar, aqui no Github na [Aba de wiki](https://github.com/dharuanluigi/dynamic-homing-pattern/wiki/Overview), o conteúdo também pode ser encontrado. Ele é basicamente um overview mais geral do que iremos encontrar aqui no repositório. Todo o processo com detalhes técnicos também estarão dentro da aba wiki aqui no guithub. Basta acessar a respectiva sessão para acessar os detalhes.

## Como usar?

Para conseguir ter a experiência completa e usar o Chatbot Sample que criei para ver como implementei o Pattern, siga as instruções abaixo:

_**Pré requisito:**_ ter uma conta na plataforma da Take Blip em https://account.blip.ai/login
E também é necessário ter noções básicas da ferramenta, que podem ser adquiridas em: https://academy.blip.ai/

1. Baixe os arquivos JSONs de dentro da pasta **Chatbot_Files;**
2. Dentro dessa pasta, você verá dois arquivos JSONs, um chamado: **dynamichomingpatternerrors** e outro chamado **dynamichomingpatternmain.**
3. Agora, basta criar um roteador e nomeá-lo como desejar.
4. Após criar o roteador, crie mais dois chatbots normais(skill) do zero, sem ser o roteador. _Sugiro dar um nome significativo para eles, pois ao decorrer do uso em determinados momentos da conversa ele vai mostrar qual é a skill que mandou a mensagem._
5. Como pode ver, nos próprios nomes dos arquivos JSONs baixados no passo 2, eles já tem um sulfixo que indica qual skill é. Basta importar cada um em uma skill que você criou no passo 4.
6. Após importar cada JSON em sua respectiva skill, basta você publicar o fluxo.
7. Ao publicar o fluxo, conecte os sub-bots no seu roteador criado no passo 3. Os serviços devem ser chamados conforme abaixo, para funcionarem sem precisar fazer alterações no fluxo:
   - **Skill principal: main** _(marcar a opção que este é meu chatbot principal)_
   - **Skill de erros: errors**

Pronto, tudo pronto para você testar a primeira implementação do Pattern.

## Lembrete

Na fase atual dessa implementação, abordo exclusivamente apenas o tipo de redirecionamento do tipo O.D.R.
