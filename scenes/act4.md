# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (game auto-saved)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *suspiro*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Ent??o, que ^caralho^ foi a moral desta hist??ria?

`hong({body:"one_up", eyes:"annoyed"})`

h: O que ?? que *aprendemos*? Eu *estava* a ser est??pido, os meus "amigos" *estavam* a usar-me, e n??s quase *morremos*.

`hong({body:"normal", eyes:"normal"})`

{{if _.harm}}
[Sim, sem mencionar a conta do hospital.](#act4a_bill)
{{/if}}

{{if !_.harm}}
[Sim, sem mencionar os danos ao f??gado.](#act4a_liver)
{{/if}}

[Sim, esse *era* o pior cen??rio poss??vel.](#act4a_worst)

[Sim, eu tinha raz??o.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Certo. Eu n??o acho que o meu seguro cobre "ser est??pido".

`hong({eyes:"annoyed", mouth:"normal"});`

b: E ainda assim... sobrevivemos!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Tenho a certeza de que reduzimos alguns anos ?? nossa vida...

`bb({eyes:"surprise"});`

b: Mas pelo menos ainda *temos* vida! N??s sobrevivemos!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: E ainda assim...

h: Hm?

`bb({eyes:"surprise"});`

b: N??s sobrevivemos!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Mas... tamb??m tinhas raz??o.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Eu *fui* o lobo que gritou lobo. Ent??o quando me deparei com perigo *real*, tu - e com raz??o - n??o acreditaste em mim.

`bb({eyes:"surprise_r"});`

b: E ainda assim... sobrevivemos!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Apesar de tudo, ainda aqui estamos.

`hong({eyes:"suspect"});`

{{if _.harm}}
h: Pareces bastante calmo, considerando que acabamos de ter uma experi??ncia de vida ou morte.
{{/if}}

{{if !_.harm}}
h: Pareces bastante calmo, considerando que acabamos de ter uma experi??ncia de vida *ou* morte.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Bem, comparado a isso, tudo o resto parece menos assustador. Tamb??m me fez pensar.

`bb({eyes:"normal", mouth:"normal"});`

b: Se o facto de eu lutar contigo ?? uma ^merda^, porque n??o te protege...

h: Mas lutar contigo *tamb??m* ?? uma ^merda^, porque s?? te faz gritar mais alto...

`bb({eyes:"normal_r"})`

b: Ent??o talvez...

`bb({eyes:"normal"})`

h: Talvez n??o seja necess??rio lutarmos.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Eu n??o sou um Lobo Mau. Mas tamb??m n??o sou um Lobo de Guarda.

`bb({eyes:"sad_d"})`

b: Eu sou um c??o de canil maltratado.

`bb({eyes:"sad"})`

b: N??s passamos por coisas dif??ceis. Talvez trauma ou neglig??ncia. ?? por isso que por vezes reajo exageradamente e penso:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: AU AU AU AU AU AU AU AU AU 

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Mas eu n??o *quero* ser um C??o Cobarde! Eu quero proteger-te! Eu quero ser um Bom C??o!

`bb({eyes:"sad", mouth:"normal"});`

b: Humano... Podes ajudar-me a domar este Lobo?

`hong({eyes:"sad"})`

h: Eu... Vou tentar.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Ok. Um relacionamento saud??vel com emo????es. Relacionamentos precisam de comunica????o. Ent??o, vamos comunicar.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Os pr??ximos cinco minutos v??o parecer super melosos, mas ?? como dizem "pr??tica leva ?? perfei????o".

```
hong({body:"hands_2", mouth:"normal"});
```

h: Querido Lobo interior ... como *est??s* a sentir-te?

n2: N??MERO TOTAL DE MEDOS USADOS:

n2: *MAGOADO* {{_.attack_harm_total}}, *N??O AMADO* {{_.attack_alone_total}}, *M?? PESSOA* {{_.attack_bad_total}}

n2: DE QUE MEDO QUERES FALAR PRIMEIRO? (PODES FALAR DOS OUTROS MAIS TARDE)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Estou com medo de sermos magoados.](#act4_harm)

[Estou com medo de ficarmos sozinhos.](#act4_alone)

[Estou com medo de que sejamos m??s pessoas.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Eu quero proteger a tua necessidade de seguran??a f??sica,

`bb({eyes:"sad_d"})`

b: Mas o *mundo* parece t??o perigoso. T??o cheio de trag??dia e maldade.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: N??o sei, chega de ser *eu* a escolher o que dizer a seguir. O que *dizes* , humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Outra vez, de volta a ti, humano. O que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais pensamentos, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Tens raz??o. Ent??o, vamos proteger-nos.](#act4_harm_skills)

[Vamos expor-nos a *mais* perigos.](#act4_harm_exposure)

[Obrigado.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Mas ... como? Tenho presas e garras, mas sou apenas uma met??fora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Podemos aprender autodefesa? Juntarmo-nos a uma comunidade onde nos protegemos uns aos outros? Melhorar a nossa sa??de geral e limites pessoais?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Talvez, mas ...

[Por onde come??amos?](#act4_harm_skills_start)

[E se ainda n??o funcionarem?](#act4_harm_skills_work)

[E se exagerarmos na "seguran??a"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: H?? tanto a fazer, tanta coisa que precisamos de consertar em n??s mesmos. Com o que *come??amos*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Estamos a come??ar agora.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ah?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Estamos a praticar boa comunica????o agora. O que nos ajudar?? a detetar melhor o perigo, com menos falsos positivos,

`hong({ eyes:"surprise" });`

h: E *isso* vai ajudar-nos a proteger contra o perigo!

`hong({ eyes:"normal", mouth:"normal" });`

h: Portanto: isto *?? um* treino de autodefesa.

`bb({ eyes:"normal_r" })`

b: Huh. Eu estava ?? espera de algo como:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Verdade, n??o h?? como nos proteger a 100%...

`hong({ body:"one_up" });`

h: Mas mesmo uma melhoria de 1% j?? vale alguma coisa, certo?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Est??s a ver o copo, n??o como 99% vazio, mas como 1% cheio?

`bb({ eyes:"normal" });`

h: O que ainda vale alguma coisa se estiveres perdido no deserto.

`bb({ eyes:"closed" });`

b: Bem. Bota abaixo, ent??o.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Quer dizer, tu s?? ignoraste os meus avisos porque *eu exagerei* com a seguran??a!

`bb({ body:"normal", eyes:"normal" })`

h: N??o, tens raz??o. Seguran??a em modera????o. Tudo em modera????o.

`bb({ eyes:"suspect" })`

b: Desculpa, *TUDO* em modera????o?

`hong({ eyes:"annoyed" })`

h: *Um n??mero moderado de coisas* em modera????o.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Obrigada por fazeres as tuas declara????es recursivamente auto consistentes.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *O QU??*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Quer dizer, digamos que um C??o tem medo da trovoada.

`hong({ body:"hands_1" });`

h: Um truque que os treinadores usam ?? tocar uma grava????o de trovoada num volume baixo e, a seguir, d??o ao c??o uma recompensa por ficar calmo.

`hong({ body:"hands_2" });`

h: Ao longo de v??rios dias, o treinador aumenta o volume aos poucos, at?? que o C??o supere o medo de trov??es.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Chama-se terapia de exposi????o!

`hong({ body:"point", eyes:"normal" });`

h: J?? que ??s um C??o, deve funcionar para ti tamb??m, certo? Todos os mam??feros t??m a mesma resposta no que toca a "luta ou fuga".

`hong({ body:"normal" });`

[E se dessensibilizarmos *demais*?](#act4_harm_exposure_overboard)

[E se estivermos expostos a um perigo *real*?](#act4_harm_exposure_hurt)

[Eu sou um Lobo, n??o um C??o.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Eu vou mostrar-te bondade e paci??ncia at?? estares domesticado e virares um c??ozinho fofinho.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Duh.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: *Acabamos* de ver o que acontece se bloqueares o teu medo - p??es-te em situa????es *realmente* perigosas.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Al??m disso, *demasiada* dessensibiliza????o n??o nos vai transformar em psicopatas?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Daqui a bocado, vamos estar a recompensar-nos enquanto vemos pornografia de "snuff"!

`hong({ eyes:"annoyed" })`

h: Eu... acho que h?? uma linha entre isso e a trovoada.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Mas *onde* exatamente, humano? *Onde?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: N??o sei. Mas *podes* ajudar-me!

`hong({ eyes:"normal", body:"normal" })`

h: Ao trabalhar e negociar contigo, conseguiremos tra??ar essa linha.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ok. Mas eu n??o tenho polegares, por isso vais ter de ser tu a desenhar.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.harm}}
b: Por exemplo: saltamos de um *telhado!*
{{/if}}

{{if !_.harm}}
b: Por exemplo: quase saltamos de um *telhado!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Nah, tens raz??o. *Podemos* ir mais longe.

`hong({ eyes:"normal" });`

h: Mas ?? por isso que, se fizermos terapia de exposi????o, come??aremos devagar e daremos pequenos passos para melhorar.

h: Antes de atingirmos o perigo *real*, paramos.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Sim, eu tra??o a linha entre ouvir um trov??o alto e ficar no meio de uma tempestade com um chap??u alto e pontiagudo.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Espera, nenhum argumento a favor ou contra o que estou a sentir? S??... "obrigado"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Sim! Obrigado por mostrares a tua preocupa????o com as minhas {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Est??s bem?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Nunca *me tinhas* agradecido antes.

`hong({ mouth:"smile" });`

h: Aw, seu grande e felpudo Lobo stressado.

(#act4_something_else)

# act4_thanks_2

h: Mesmo que reajas de forma exagerada, agrade??o por cuidares do meu {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Espera... n??o est??s s?? a repetir "obrigado" para evitar realmente falar sobre esses medos, ou est??s?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Bem, as coisas s??o complicadas e nem sempre tenho as respostas prontas.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: N??o ?? como se a vida nos desse uma lista de 3 respostas de di??logo predefinidas.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Mas, por agora, posso pelo menos dizer obrigado.

b: Bem, obrigado tamb??m por me ouvires t??o pacientemente.

`bb({ eyes:"closed" });`

b: Seu pequeno e careca mam??fero.

(#act4_something_else)

# act4_thanks_3

h: Mesmo que os teus latidos me assustem, sei que est??s apenas a tentar proteger-me {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Ok, se continuares a elogiar-me assim, a internet vai ficar com algumas ideias estranhas sobre n??s.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Por amor de Deus, sou apenas um beb?? universit??rio vulner??vel e tu ??s um Lobo grande e assustador. O que ?? o pior que pod-

`hong({ eyes:"normal", body:"point" });`

h: Na verdade, n??o respondas a isso.

(#act4_something_else)



# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Eu quero ter a certeza de que preenches a tua necessidade de pertencer...

`bb({ eyes:"sad_u" });`

b: Mas preocupa-me que, caso algu??m nos conhe??a - o *verdadeiro* n??s - se assustem connosco.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: N??o sei, chega de ser *eu* a escolher o que dizer a seguir. O que *dizes* , humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Outra vez, de volta a ti, humano. O que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais pensamentos, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Concordo: vamos trabalhar na nossa vida social.](#act4_alone_skills)

[Acho que as pessoas gostam de n??s. Vamos descobrir?](#act4_alone_experiment)

[Obrigado.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Poder??amos praticar habilidades como fazer perguntas, ouvir e ter empatia, ser aberto e vulner??vel, etc?

`hong({ eyes:"normal_l" });`

h: Ou criar h??bitos sociais melhores, como planear qualquer coisa com amigos ou sair regularmente?

`hong({ body:"one_up" });`

h: Tamb??m poder??amos aprender a ficar mais confort??veis com rejei????o.

`hong({ eyes:"normal" });`

h: Ou aprender a saber quando as pessoas *n??o* nos est??o a rejeitar, est??o apenas cansadas ou t??m Resting ^Bitch^ Face.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: H?? muitas op????es. Mas, sobre "aprender habilidades sociais"...

[Isso n??o ?? *manipulador?*](#act4_alone_skills_manipulative)

[N??o nos tornar?? *mais f??ceis de manipular?*](#act4_alone_skills_manipulated)

[E se falharmos?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Os serial killers que podem ler as emo????es das v??timas n??o s??o ??timos com "empatia"?

`bb({ eyes:"annoyed" });`

b: O Charles Manson n??o arranjou amigos e influenciou pessoas?

`hong({ eyes:"annoyed", body:"chin" });`

h: N??o, tens raz??o.

h: "Habilidades sociais" n??o significam nada se n??o quisermos, genuinamente, saber *das* pessoas.

`hong({ body:"normal" });`

h: Basicamente, basta n??o ser ^imbecil^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Est?? a?? uma magnifica frase para um p??ster motivacional.

`hong({ body:"shrug", mouth:"narrow" });`

h: ???N??o sejas ^Imbecil^ ??????

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Vamos tornar-nos tapetes de boas-vindas, a dizer "por favor" e "obrigado" enquanto as pessoas limpam os p??s em n??s!

`bb({ mouth:"scream", eyes:"scream" })`

b: Vamos lamber tantas botas, vai parecer que estamos usar graxa nos l??bios!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: N??o, tens raz??o. "Habilidades sociais" n??o pode ser apenas para agradar aos outros, tamb??m serve para estabelecer *limites.*

`hong( body:"one_up" });`

h: N??o podemos convidar outras pessoas para a nossa casa, se n??o tivermos paredes para sustent??-la.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: J?? agora...: aquela imagem mental dos l??bios... *ew??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Podemos falhar. Na verdade, *iremos* falhar.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Mas n??o h?? problema! Fracassar ?? como se aprende!

`hong({ body:"normal", eyes:"normal" });`

h: Ent??o, vamos avan??ar juntos, ok?

`bb({ eyes:"normal_r" });`

b: Claro, acho... na pior das hip??teses, podemos simplesmente fugir da cidade e arranjar uma identidade nova.

`bb({ eyes:"normal" });`

h: Sim, acho que isso s?? custa duas bitcoins hoje em dia.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Pod??amos fazer algumas exper??ncias!

`hong({ body:"chin" });`

h: Pod??amos enviar um ping a um amigo para sair, reconectar com um colega ou at?? conversar com o barista.

`hong({ body:"normal" });`

h: Acho que vamos descobrir que somos mais simp??ticos do que pensamos.

`bb({ eyes:"annoyed" });`

[E se essas forem "vit??rias" pequenas?](#act4_alone_experiment_cheap)

[E se isso for inconveniente para os outros?](#act4_alone_experiment_burden)

[Mas conversa fiada n??o ?? o "*verdadeiro* n??s"!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se pusermos um sorriso falso, nunca vamos realmente conectar-nos com ningu??m,

`bb({ eyes:"super_sad" });`

b: *Mas* se nos abrirmos, as outras pessoas ir??o ver as nossas entranhas!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Rebola.

b: O qu??.

`hong({body:"hands_1"})`

h: Quando os c??es querem mostrar amor e confian??a, eles tornam-se vulner??veis ao exp??r a barriga.

`hong({body:"one_up"})`

h: Talvez *ainda* n??o estejamos seguros o suficiente para sermos muito vulner??veis, mas com treino suficiente,

`hong({body:"normal", eyes:"surprise"})`

h: Um dia podemos mostrar ??s pessoas quem somos na realidade - todos confusos, todos humanos.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Vou rebolar se me deres mimos.

`bb({ eyes:"normal", mouth:"normal" });`

h: N??o.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dizer "Ol??" ao barista n??o ?? exatamente o desempenho de medalha de ouro nas Olimp??adas das Borboletas Sociais.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Para *n??s ??!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: Na ??rea social, nem do escal??o dos "featherweight" somos, somos como... "quark-weight".

`hong({ body:"normal", eyes:"normal" });`

h: Se tivermos de come??ar com vit??rias pequenas, assim seja. H?? que subir o primeiro degrau antes do mil??simo degrau.

b: Sim! Talvez depois de dizer "Ol??", possamos avan??ar para um...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Tudo bem?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Sim e contigo!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Talvez o barista s?? queira fazer o raio do caf?? e n??o fazer parte de uma *experi??ncia* para ver se nossas habilidades sociais s??o m??s.

`bb({ eyes:"annoyed" })`

h: Bem, se for ??bvio que *somos* um inconveniente...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: ?? bom que o saibamos tamb??m!

`hong({ eyes:"normal" });`

h: Mais tarde podemos aprender a perguntar proativamente ??s pessoas aquilo com que se sentem confort??veis, para saber e respeitar os limites delas.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Tu sabes, aquela ^merda^ de "habilidades interpessoais" que vemos nos panfletos.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Eu quero defender as tuas necessidades morais, essa vontade de ter tornares uma pessoa melhor,

`bb({ eyes:"sad_d" })`

b: Mas parece que, no fundo, estamos fundamentalmente... despeda??ados.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.harm}}
b: E n??o me digas que *n??o* estamos confusos. Saltamos de um *telhado*.
{{/if}}

{{if !_.harm}}
b: E n??o me digas que *n??o* estamos confusos. Quase saltamos de um *telhado*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: N??o sei, chega de ser *eu* a escolher o que dizer a seguir. O que *dizes* , humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Outra vez, de volta a ti, humano. O que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais pensamentos, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ent??o estamos despeda??ados. Vamos consertar-nos.](#act4_bad_fix)

[Ent??o estamos despeda??ados. Vamos aceitar isso.](#act4_bad_accept)

[Obrigado.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Podemos ir construindo h??bitos melhores, colocar a nossa vida mais alinhada com o que valorizamos,

`hong({body:"one_up"});`

h: E se for necess??rio, podemos arranjar ajuda profissional - um terapeuta ou conselheiro.

`hong({body:"normal"});`

h: Existem maneiras de nos consertar.

[E se n??o conseguirmos consertar tudo?](#act4_bad_fix_cant)

[E se consertarmos em *demasia*?](#act4_bad_fix_too_much)

[N??o podemos pagar ajuda profissional.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: N??o, acho que tens raz??o.

h: N??o podemos consertar tudo.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh eu sabia que ficar??amos despeda??ados para sempre!

`hong({eyes:"surprise"});`

h: Mas podemos, pelo menos, ser "n??o *t??o* " despeda??ados.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: As cicatrizes curam com o tempo, mas nunca desaparecem. E n??o h?? problema.

`bb({eyes:"annoyed_r"});`

b: Talvez. Al??m disso,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Cicatrizes s??o *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Por favor, n??o fa??as isso.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: ?? doentio admitir, mas... parte de mim *quer* ter este transtorno.

`bb({ eyes:"angry" })`

b: Quer dizer, sem ele, n??o ser??amos *aborrecidos?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Sem a desordem, a nossa arte n??o se tornaria obsoleta e sem gra??a?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Sem o transtorno, n??o ser??amos incapazes de nos conectar com os nossos amigos que t??m o transtorno?

`bb({ eyes:"sad", body:"chest" })`

b: Se estivermos sempre contentes com a vida, n??o vamos parar de nos esfor??ar para fazer coisas extraordin??rias?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se tivermos medo de ... "esgotar os nossos medos" ...

h: Eu n??o acho que vamos ficar sem medos.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, sim! Ufa! Que alivio!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doutor, estou ansioso por pagar 100??? ?? hora s?? para o ouvir perguntar "*Como ?? que isso te faz sentir"?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E como ?? que isso te faz sentir?

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, essa ?? uma preocupa????o totalmente razo??vel.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E ?? realmente uma pena que a sa??de mental n??o seja acess??vel para muitas pessoas.

`hong({ eyes:"normal", mouth:"normal" });`

h: Ainda assim, existem algumas op????es baratas ou gratuitas:

`hong({ body:"chin" })`

h: Grupos de apoio, terapia online, centros de sa??de estudantis / sem fins lucrativos...

`hong({ body:"hands_1" })`

h: Construir h??bitos como medita????o, dormir bem, conversar regularmente com amigos, aprender coisas novas ...

`hong({ body:"hands_2" })`

h: Ir ?? biblioteca buscar livros de exerc??cios para psicoterapias baseadas em evid??ncias ...

`hong({ body:"one_up" })`

h: H?? uma lista completa de recursos no final deste jogo!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Bem, *esta* "fourth wall" n??o durou muito.

`hong({ body:"point" });`

h: Algumas coisas s??o mais importantes do que a conven????o narrativa. Como a sa??de mental.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Quer dizer, ?? isso que dizem os terapeutas, certo? Aceita todas as tuas emo????es, mesmo as negativas?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Espera.

["Aceitar" como em *desistir*?](#act4_bad_accept_give_up)

["Aceitar" como em *aprov??-las*?](#act4_bad_accept_approve)

["Aceitar" como em lev??-las *a s??rio*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Achas que o Martin Luther King teria dito: "?? uma ^merda^ n??o nos podermos sentar na parte da frente do autocarro, mas vamos s?? *aceitar* ?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Por que ?? que o Complexo Industrial de Autoajuda acha que acenar a bandeira branca ?? *sabedoria profunda?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Eu acho que os terapeutas querem dizer "aceitar" coisas m??s como em: reconhecer que existem e s??o dif??ceis de mudar,

h: Mas n??o necessariamente desistir de um compromisso com a mudan??a.

`bb({ eyes:"suspect" });`

b: Ent??o os terapeutas devem dizer *reconhecer*, n??o *aceitar*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Sim, pensando bem, "aceitar" ?? meio confuso.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Bem, eu *reconhe??o* isso.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Como ?? *bom* estarmos despeda??ados ou algo assim? N??o!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Todos aqueles argumentistas de Hollywood que romantizam doen??as mentais est??o cheios de ^merda^ na cabe??a!

`bb({ eyes:"angry", body:"two_up" });`

b: Ter um transtorno mental ?? uma ^*merda^!* Rouba *vida ??s pessoas!* Porque ?? que devemos "aceitar" isso?!

`bb({ body:"normal" });`

h: Acho que terapeutas querem dizer "aceitar" as nossas emo????es como em: sejam pacientes com elas.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Por exemplo, da mesma maneira que nos mexermos em areia movedi??a nos faz afundar mais r??pido, e a solu????o ?? ficar pacientemente quieto,

`hong({ eyes:"surprise" });`

{{if _.harm}}
h: Lutar contra ti, o meu medo, levou-me a saltar de um telhado.
{{/if}}

{{if !_.harm}}
h: Lutar contra ti, o meu medo, quase me levou a saltar de um telhado.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Em vez disso, a solu????o ?? fazer o que estamos a fazer agora - n??o lutar, mas estar pacificamente um com o outro.

`bb({ eyes:"annoyed" });`

b: Ent??o eles deviam dizer *isso* em vez de uma palavra t??o problem??tica como "aceitar".

`hong({ body:"chin", eyes:"annoyed" });`

h: Sim, pensando bem, "aceitar" ?? uma ^merda^.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: N??o aceito "aceitar".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Mas j?? *sabemos* que n??o deves levar-me a s??rio!

`bb({ eyes:"sad_u", body:"two_up" });`

b: O *problema* ?? que eu quero ajudar-te, mas sou p??ssimo a usar palavras para fazer isso!

`bb({ eyes:"sad", body:"normal" });`

h: Acho que os terapeutas querem dizer "aceitar" as emo????es como em: "n??o lutes com elas nem as ignores".

`hong({ eyes:"surprise", body:"one_up" });`

h: Para te ouvir, trabalhar *contigo* , mas n??o tomar o que dizes como uma verdade 100% literal.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Ent??o os terapeutas deviam dizer *isso* em vez de uma palavra t??o confusa e vaga como "aceitar".

`hong({ body:"chin", eyes:"annoyed" });`

h: Eu acho que eles s??o p??ssimos no que toca ao uso de palavras.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Enfim, queres falar de mais alguma coisa?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Ent??o, h?? mais alguma coisa a pesar nesse teu cora????o?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Estou com medo de sermos magoados.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Estou com medo de ficarmos sozinhos.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Estou com medo de que sejamos m??s pessoas.](#act4_bad)
{{/if}}

[Nah, estou bem por agora.](#act4c_prelude)

# act4_something_else_2

h: Ok, acho que j?? falamos sobre todos os nossos medos.

b: Sim, existem apenas tr??s medos.

h: Sim, exatamente, tr??s.

b: Conveniente.

(#act4c)

# act4c_prelude

h: Boa conversa equipa.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Isto n??o ?? um *jogo*, sabes.

`bb({eyes:"angry_d", body:"one_up"})`

b: Construir um relacionamento saud??vel com as tuas emo????es n??o ?? t??o simples como clicar em bot??es numa tela.

`bb({eyes:"sad", body:"normal"})`

b: *Podemos* mesmo dar-nos bem?

b: *Podemos* trabalhar juntos, como uma equipa?

`hong({eyes:"sad", body:"one_up"})`

h: Bem,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: C-com licen??a ...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: I-i-importas-te que me sente contigo para almo??ar?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *?? este* o teu crush? Por que est?? sentado sozinho como um psicopata?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: A perguntar ao teu crush se te podes sentar com ele? Tens no????o do qu??o *carente* pareces?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *?? este* o teu crush? Interrompemos paz e sossego dele! Somos t??o inconvenientes!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Q-q-quer dizer- es-est?? tudo bem se n??o puder, eu s??...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Espera, n??o te vi na festa?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Sim, claro! Vem c??.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Desculpa, preciso de um tempo sozinho agora.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sim, estavas no sof??! Na primeira festa a que fui...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Onde tive aquele ataque de p??nico e dei um soco ao anfitri??o.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Onde tive aquele ataque de p??nico e fugi a chorar.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera, humano, podemos estar a deix??-la desconfort??veis.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, n??o ?? a minha inten????o deix??-la desconfort??vel!

`publish("act4", ["hong_to_alshire",4]);`

h2: Estou apenas a relembrar-me de um rosto amigo, s?? isso.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH EU SABIA! ALERTA: PSICOPATA PERIGOSO EM P??NICO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH A PRIMEIRA IMPRESS??O QUE FIZEMOS FOI "TESTEMUNHASTE O MEU TRAUMA"! Isso significa que nos odeia!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH FIZEMOS ALGU??M LEMBRAR-SE DE UM EVENTO TRAUM??TICO. S?? A NOSSA PRESEN??A J?? MAGOA OS OUTROS.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera, humano, ela parece desconfort??vel.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, sem press??o, ?? claro!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Podes sentar-te aqui se quiseres.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: EST?? A SER *DEMASIADO* AMIG??VEL! IGUALZINHO AO TED BUNDY, O ASSASSINO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: EST?? S?? A FINGIR SER SIMP??TICO! NINGU??M QUER, *REALMENTE* , ESTAR PERTO DE N??S!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH N??S FAZEMOS SEMPRE OS OUTROS SENTIREM-SE ESQUISITOS! SOMOS T??O DESAGRAD??VEIS!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera, humano, podemos estar a deix??-la desconfort??vel.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, n??o quero ser rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: S?? preciso de algum tempo para processar as minhas emo????es. Por favor, n??o leves isto como uma rejei????o pessoal.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: QUE PENSAMENTOS DOENTIOS E TORCIDOS EST?? A PROCESSAR?! QUE DESEJOS OBSCUROS PREENCHEM O CORA????O DESTE PSICOPATA?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: FOMOS REJEITADOS! NUNCA SEREMOS AMADOS!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: INTERROMPEMOS O PROCESSAMENTO EMOCIONAL DELE! AGORA EST?? TRAUMATIZADO PARA SEMPRE E ?? TUDO CULPA NOSSA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: FOGE FOGE FOGE FOGE FOGE FOGE FOGE FOGE FOGE FOGE

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. Aquilo foi estranho. Pergunto-me o que estava a passar-lhe pela cabe??a.

`publish("act4", ["hong_closer", 2]);`

h: Enfim, o que estavas a dizer?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, esqueci-me? Algo sobre equipas e trabalho?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ??\_(???)_/??

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Dizem que deves "fazer as pazes" com as tuas emo????es, como se as tuas emo????es fossem *criminosos*.

`publish("act4", ["bb_closer", 7]);`

b: Mas eu quero ter *mais* do que mera paz! Eu quero que sejamos *aliados!*

`publish("act4", ["bb_closer", 3]);`

b: Eu quero ser um bom C??o de Guarda. Assim como a fome e a sede s??o alarmes para as tuas necessidades f??sicas,

`publish("act4", ["bb_closer", 8]);`

b: Eu quero ser o alarme para as tuas necessidades *psicol??gicas* - as tuas necessidades de seguran??a, pertencimento, bondade.

`publish("act4", ["bb_closer", 1]);`

b: Mas... Eu sou p??ssimo no meu trabalho, ent??o preciso que me treines.

`publish("act4", ["bb_closer", 4]);`

b: N??o sou "sempre v??lido", nem "sempre irracional". Estou apenas ... a dar o meu melhor. Ent??o, por favor???

`publish("act4", ["bb_closer", 30]);`

b: Ajuda-me a ajudar-te!

`publish("act4", ["bb_closer", 6]);`

b: Por??m, ensinar truques novos a um c??o velho *vai* demorar um pouco. Talvez *anos.*

`publish("act4", ["bb_closer", 3]);`

b: E por vezes vou ter uma reca??da, vou cair nos meus velhos h??bitos.

`publish("act4", ["bb_closer", 2]);`

b: Vou latir a sombras. Vou assustar-te com palavras. Posso at?? mostrar-te algumas imagens intrusivas de... coisas.

`publish("act4", ["bb_closer", 9]);`

b: Desculpa. Eu sou um c??o de canil maltratado. C??es maltratados fazem coc?? na tua cama de vez em quando!

`publish("act4", ["bb_closer", 4]);`

b: Mas se fores paciente comigo... e te "sentares" comigo...

`publish("act4", ["bb_closer", 8]);`

b: Talvez possas domar este Lobo.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[C??o lindo.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Humano lindo.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA AINDA EST??S A COMER SOZINHO! QUINZE CIGARROS AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA AINDA N??O FOSTE PRODUTIVO ENQUANTO COM??AMOS, SOMOS PARASITAS DA SOCIEDADE AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA EST??S A COMER MAIS P??O BRANCO AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: AU AU AU AU AU AU AU AU AU 

(#credits)
