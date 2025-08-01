---
title: Testando em Prod - Patos de Borracha
---

A área de tecnologia, como muitas outras áreas, possui um folclore próprio – com histórias, mitos e tradições que se perpetuaram ao longo dos anos através da oralidade e, é claro, da internet. Uma ideia que habita o imaginário de muitos devs é a do pato de borracha. Dizem que ao estar batendo cabeça com um bug no código, você pode explicar cada parte dele para um pato de borracha em voz alta e, eventualmente, o problema vai saltar nos seus olhos. Eu, particularmente, nunca falei com nenhum pato de borracha e nem conheço quem tenha feito isso. A origem do rubber duck debugging (depuração/debug do pato de borracha) surge no livro The Pragmatic Programmer, de Andrew Hunt e David Thomas e defende a ideia de que explicar linha a linha do código obriga o programador a analisar de forma mais crítica aquilo que escreveu. Os estadunidenses parecem ter menos traquejo social do que nós, brasileiros, que geralmente optamos por abordar um colega ao invés de ficar falando com um objeto inanimado.

Atualmente, em um mundo onde as IAs generativas dominaram o ambiente de trabalho, surge uma pergunta: onde foram parar os patos de borracha?

Uma das coisas que sempre me chamou atenção na área de tecnologia é o senso de comunidade. Programadores gostam de construir coisas e, não só isso, gostam de compartilhar aquilo que constroem. Eu não sei você, mas eu não conheço nenhuma outra área onde profissionais estão dispostos a contribuir para projetos sem receber um centavo por isso – apenas pela satisfação pessoal de estarem ajudando a construir algo que acham interessante.
Não por acaso, grandes projetos de software tiveram um rápido crescimento graças ao movimento open source – projetos de código aberto nos quais qualquer um pode participar. O Linux talvez seja um dos exemplos de maior sucesso. O que começou com um projeto pessoal de um jovem finlandês conta hoje com mais de 15.000 desenvolvedores atuantes espalhados pelo mundo.

Esse espírito de comunidade também é forte quando o assunto é ajudar pessoas a resolverem problemas ou a sanar dúvidas.

Talvez seja por isso que o StackOverflow, site de perguntas e respostas voltadas para programação, fez tanto sucesso na segunda década dos anos 2000.

Está tendo problemas para usar uma biblioteca? A instalação de um SDK está quebrando? Seu código não compila? Sua API só retorna 500? Bastava postar sua dúvida e em minutos alguém apareceria para responder: fosse para compartilhar, dentro de sua experiência pessoal, como resolveu o problema, ou só para mandar o link da documentação e dizer em tom de poucos amigos “read the docs”.

Acontece que não demorou muito para que o sistema de up vote e down vote, junto com a atribuição de pontos aos perfis, tornasse o site um pouco hostil, sobretudo para novatos. Pouco a pouco, criou-se um esteriótipo do tipo de desenvolvedor que participava ativamente das discussões: gente com muita experiência e conhecimento em certas áreas, o que costumava vir acompanhado de um ar de superioridade e uma certa arrogância. Respostas ofendendo a capacidade de quem estava perguntando já não eram surpresa, mas sim só mais uma terça-feira comum.

Quando, em 2022, a OpenAI anuncia o ChatGPT, a hipótese do impacto que isso teria em sites de perguntas e respostas foi levantada e, portanto, não foi surpresa o início de uma queda expressiva nas postagens no StackOverflow com a ascensão da mais nova atração do momento. A plataforma saiu de um pico de cerca de 80 mil postagens em abril de 2023 para menos de 20 mil em maio de 2025.

Como isso afeta o meio de tecnologia?

Nós podemos olhar para o assunto através de diferentes recortes. Alguns desses recortes, inclusive, têm sido esgotados em amplas discussões. Desde o aumento de bases de código geradas por IAs indo para produção – e a possibilidade de uma quebra em muitos sistemas em um médio prazo (o dilema do vibe coding) – até um prejuízo no senso crítico e na resolução de problemas por parte de devs que se limitam a escrever prompts.

Porém, me interessa um recorte mais social: a subjetividade da troca de experiência está sendo comprometida.

Da mesma forma que a gente dá ctrl+c, ctrl+v em um trecho de código que o ChatGPT gera, também era assim que fazíamos com os trechos de códigos nas respostas do StackOVerflow, com a diferença de não existir mais uma discussão sobre o problema em si.

Como diz o outro, “nenhuma experiência é singular” e se tem uma coisa que IAs não possuem é experiência pessoal. A medida que o volume de dados para treinar os modelos cresce, também crescem as possibilidades que o agente pode considerar, mas, pelo menos nesse momento, a subjetividade debilitada dessas ferramentas produz, na maioria dos casos, respostas genéricas. Não só isso, a troca dentro de uma comunidade nunca se limita ao assunto original – sempre tem alguém fazendo associações ou trazendo referências que enriquecem a discussão.

Para uma pergunta que fulano fizesse, ciclano e beltrano dariam soluções diferentes e mais uma galera ia acrescentar seus dois dedos de prosa pra complementar o que estava sendo proposto.

A medida que novos agentes são lançados, eu noto que um movimento de clausura surge: você só precisa de um editor de texto e uma IA generativa para criar o próximo micro-sass que vai expor os dados de todos os usuários por conta das brechas de segurança que a IA não levou em conta quando cuspiu o código para você.

O que nos leva a um outro problema: código. Deixa eu contar uma história rápida.

No começo da faculdade ainda, eu consegui um estágio. Cheguei com sangue no olho, doido para codar e mostrar todas as minhas habilidades (que eram bem limitadas, naturalmente). Eu comia código com feijão e farinha, no café, almoço e jantar. Eu sonhava com código, respirava isso constantemente. Um dia, em uma reunião com o dev responsável por me orientar, estávamos discutindo uma task. Eu atropelei ele e comecei a falar sobre como eu ia implementar a solução, até que ele virou para mim e perguntou: que solução? Eu congelei por um segundo e aprendi a primeira lição importante dentro da minha carreira de desenvolvedor. O que eu ouvi desse dev foi o seguinte: você está muito focado no código que você vai escrever, sendo que você nem entendeu o problema que está tentando resolver.

No cenário atual, vai se construindo uma falsa ideia de que tudo é mais fácil do que realmente é, e nós esquecemos da importância de fazer a lição de casa. Conversar com gente, nos faz lembrar disso.

Voltando a pergunta inicial: os patos de borracha se tornaram agentes de IA, com respostas prontas (nem sempre certas), bem como códigos prontos (nem sempre certos). A ideia do rubber duck debugging foi comprometida, porque o senso crítico vai morrendo cada vez que nós escrevemos “não funcionou” para uma resposta que a IA nos deu.
