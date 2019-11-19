## Adicionando um cronômetro

Vamos adicionar um cronômetro a seu jogo para que o jogador tenha que chegar à ilha o mais rápido possível.

--- task ---

Adicione uma nova variável chamada `tempo`{:class="block3variables"} ao Palco.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Você também pode escolher um visual para seu cronômetro, alterando a forma como sua nova variável é exibida.

--- /task ---

--- task ---

Agora adicione blocos de código ao Palco para que o cronômetro faça contagem do tempo até que o barco chegue à ilha.

--- hints ---
 --- hint --- No Palco, `quando a bandeira verde for clicada`{:class="block3control"}, `atribua 0 para a variável tempo`{:class="block3variables"}. Dentro da repetição `sempre`{:class="block3control"}, você primeiro precisa `espere 0.1 segundos`{:class="block3control"}, então `adicione 0.1 a tempo`{:class="block3variables"}.
--- /hint ---
 --- hint --- Aqui estão os blocos que você vai precisar: ![stage](images/stage.png)

```blocks3
adicione (0.1) a [tempo v]

quando ⚑ for clicado

sempre
end

espere (0.1) seg

mude [tempo v] para [0]
```

--- /hint --- --- hint --- Seu código deve ficar assim: ![stage](images/stage.png)

```blocks3
quando ⚑ for clicado
mude [tempo v] para [0]
sempre 
 espere (0.1) seg
 adicione (0.1) a [tempo v]
fim
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Teste seu jogo e veja quão rapidamente você pode levar o barco para a ilha!

![screenshot](images/boat-variable-test.png)

--- /task ---