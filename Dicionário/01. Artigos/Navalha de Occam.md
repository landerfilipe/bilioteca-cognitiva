---
titulo: "[[Navalha de Occam]]"
categoria: Epistemologia
tags:
  - parcimônia
  - subdeterminação
  - indução
  - seleção-de-modelos
  - inferência-bayesiana
  - falseabilidade
  - sobreajuste
data: 23 de junho de 2026
modelo: Opus 4.8
resumo: Entre explicações que dão conta igualmente bem dos mesmos fatos, prefira a que postula menos entidades. Não é um critério de verdade, mas uma regra de aposta — a hipótese mais econômica é o melhor ponto de partida, nunca a sentença final sobre o mundo.
---
---
# Navalha de Occam

## O problema

==Qualquer conjunto finito de observações é compatível com um número infinito de explicações.== Esta não é uma fragilidade ocasional do conhecimento; é a condição estrutural de toda inferência empírica, e tem nome técnico: a **[[subdeterminação]]** da teoria pelos dados. Passe uma reta por dois pontos e ela os atravessa perfeitamente — mas uma parábola também passa, e uma senoide, e uma curva de grau dez que serpenteia entre eles antes de tocá-los. Os dados não escolhem. Eles ficam quietos enquanto explicações concorrentes disputam o direito de tê-los gerado.

O mesmo vale para a defesa de uma teoria contra o fato que a contraria. Nenhuma hipótese precisa morrer diante de um contraexemplo: basta acrescentar uma suposição auxiliar que absorva a anomalia. A órbita de um planeta não fecha como previsto? Postule um epiciclo. O novo dado ainda escapa? Postule outro. O sistema de Ptolomeu sobreviveu mais de mil anos exatamente assim — não por estar certo, mas por ser **infinitamente remendável**. Toda teoria pode ser salva da refutação ao preço de ficar mais carregada de engrenagens *ad hoc*.

É aqui que mora a tensão funcional. Se qualquer explicação pode ser blindada por acréscimo, e se infinitas explicações se ajustam ao mesmo dado, então a evidência sozinha **nunca termina a discussão**. Falta um critério que não venha dos dados — uma regra de preferência que sirva de freio à multiplicação indefinida de suposições e de desempate entre rivais empiricamente equivalentes. A **navalha de Occam** é esse freio. Ela não descobre a verdade; ela impede que a explicação cresça sem necessidade e oferece um motivo principiado para escolher, entre adequações iguais, por onde começar a apostar.

## A ideia central

A formulação clássica diz: **não se devem multiplicar as entidades além da necessidade**. Diante de explicações que prestam igual conta dos mesmos fatos, prefira aquela que exige menos suposições, menos tipos de coisa, menos peças móveis. Não invente o que você não precisa inventar.

Convém uma honestidade histórica logo de início, porque a lenda em torno da navalha é maior que o documento. A frase latina que todo mundo cita — *entia non sunt multiplicanda praeter necessitatem* — **não aparece nos escritos de Guilherme de Ockham**. Ela foi cunhada séculos depois, atribuída a comentadores como João Punch, no século XVII. O que o frade franciscano efetivamente escreveu, no início do século XIV, foram variantes como *frustra fit per plura quod potest fieri per pauciora* — em vão se faz por muitos o que se pode fazer por poucos (Ockham, c. 1320). A ideia é dele; o slogan é póstumo. Quem invoca a navalha como se fosse uma sentença literal de Ockham já cometeu, na largada, o tipo de imprecisão que ela deveria coibir.

O ponto que a versão popular quase sempre amputa é a cláusula mais importante de todas: **explicações que prestam igual conta dos mesmos fatos**. A navalha só opera entre *empates explicativos*. Ela não autoriza preferir o simples-e-errado ao complexo-e-certo. Ela não diz que a realidade é simples. Diz apenas que, quando duas histórias explicam exatamente a mesma coisa e uma carrega bagagem ontológica extra que não faz trabalho nenhum, a bagagem extra é peso morto — e peso morto se corta. A navalha é, antes de tudo, uma **regra de aposta sob igualdade de evidência**, não um oráculo sobre como o mundo foi construído.

## As peças

O mecanismo tem quatro papéis, e confundi-los é a origem de quase todo mau uso.

O primeiro papel é o **corpo de evidências** que as explicações disputam — e, junto dele, a *pré-condição* que ativa toda a engrenagem: a **adequação explicativa igual**. A navalha só tem o que cortar quando as hipóteses rivais já empataram na capacidade de dar conta dos dados. Enquanto uma explica melhor que a outra, não há empate, e não há navalha: vence a que explica melhor, simples ou não. A parcimônia entra depois que o ajuste se iguala, não antes.

O segundo papel cabe às **hipóteses concorrentes** propriamente ditas — as histórias rivais sobre o que produziu os dados. Elas precisam ser genuínas competidoras pelo mesmo fenômeno, não respostas a perguntas diferentes disfarçadas de rivais.

O terceiro papel é o das **entidades** que se contam ao medir economia — e aqui há uma bifurcação que a tradição filosófica leva a sério. A *parcimônia ontológica* conta **tipos de coisa postulados**: quantas categorias novas de entidade a explicação traz ao mundo (um fluido calórico, um éter, uma força nova). A *parcimônia sintática* ou estrutural conta **suposições e parâmetros livres**: quantos botões a teoria precisa ajustar para encaixar nos dados. São cortes diferentes. Uma teoria pode ser ontologicamente enxuta e estruturalmente barroca, ou o inverso. A navalha moderna, sobretudo em estatística, mira quase sempre a segunda — o número de **parâmetros livres**.

O quarto papel, o mais escorregadio, é a própria noção de **simplicidade**. Ela não é absoluta: depende da linguagem em que a teoria está escrita. O que parece uma suposição única num vocabulário pode desdobrar-se em três noutro. Esse caráter relativo da simplicidade — a quem ela parece simples, e descrita em que termos — é o calcanhar do mecanismo, e a seção [[#Os limites|sobre os limites]] volta a ele com a faca afiada.

## A mecânica

Por que, afinal, preferir o mais simples *deveria* funcionar? A resposta intuitiva — "porque é mais elegante" — é estética e não convence ninguém. A resposta forte é que a navalha **cai automaticamente de dentro da [[inferência bayesiana]]**, sem precisar ser postulada à parte. Ela não é um princípio extra colado por fora do método; é uma consequência da aritmética da probabilidade. Esse resultado é conhecido como a **navalha de Occam bayesiana** (Jefferys e Berger, 1992; MacKay, 2003).

O raciocínio gira em torno de uma quantidade chamada **evidência do modelo** (*model evidence*) ou **verossimilhança marginal**:

$$P(D \mid M) = \int P(D \mid \theta, M)\, P(\theta \mid M)\, d\theta$$

Decomponha termo a termo. **P(D | M)** é a probabilidade que o modelo *M* atribui aos dados *D* que de fato observamos — o número que vai julgar o modelo. **P(D | θ, M)** é a [[verossimilhança]]: o quão bem o modelo prevê os dados *quando seus parâmetros θ estão fixados num valor específico*. **P(θ | M)** é a probabilidade que o modelo distribui, *antes de ver os dados*, sobre cada configuração possível de seus parâmetros. E a **integral** soma esse produto sobre todos os valores de parâmetro que o modelo admite — ou seja, faz o modelo "votar" com toda a sua gama de comportamentos possíveis, e não apenas com o ajuste mais favorável.

A consequência é o coração de tudo. Um modelo precisa **espalhar uma probabilidade total fixa — igual a um — sobre todos os conjuntos de dados que ele é capaz de prever**. Um modelo complexo, com muitos parâmetros livres, consegue prever uma enorme variedade de dados possíveis; portanto sua probabilidade se reparte fininha sobre esse território vasto. Um modelo simples prevê poucos resultados; concentra a aposta. Quando os dados realmente observados caem dentro do que ambos previam, o modelo simples — que apostou concentrado e acertou — atribui a eles **probabilidade maior** do que o modelo complexo, que dilui sua aposta por dispersá-la entre mil futuros que não aconteceram. O complexo é punido não por ser falso, mas por ser **vago de tanto ser flexível**.

Um exemplo trabalhado torna o número palpável. Imagine dois modelos para uma sequência observada de dados. A **Teoria A** afirma: a sequência tem de ser *exatamente esta*. A **Teoria B** afirma: a sequência pode ser qualquer uma entre mil padrões igualmente possíveis. As duas são compatíveis com o que se viu — nenhuma é refutada pela observação. Mas A concentrou toda a sua probabilidade naquele único resultado, atribuindo-lhe valor 1; B repartiu sua probabilidade por mil candidatos, sobrando 1/1000 para o que de fato ocorreu. A razão de evidência entre elas é de **mil para um a favor da teoria mais restritiva**, e isso emerge sozinho da conta, sem nenhum apelo à elegância. A teoria que se compromete mais — que se arrisca mais a errar — é recompensada quando acerta. Esta é, não por acaso, a ponte com a **[[falseabilidade]]**: Popper já argumentava que teorias mais simples são mais testáveis porque proíbem mais, expondo-se mais ao risco de refutação e, com isso, dizendo mais sobre o mundo (Popper, 1959).

Há uma segunda formalização da mesma intuição, vinda da teoria da informação: o **comprimento mínimo de descrição** (*Minimum Description Length*). A regra manda escolher o modelo que minimiza a soma de duas parcelas — **o custo de descrever o modelo** mais **o custo de descrever os dados usando esse modelo** (Rissanen, 1978), ideia enraizada na complexidade algorítmica de Kolmogorov e Solomonoff (Kolmogorov, 1965). Um modelo trivial é barato de descrever, mas deixa muito resíduo nos dados; um modelo barroco descreve os dados sem sobra, mas é caríssimo de enunciar. O ótimo fica no meio: a descrição **mais curta no total** costuma ser a que captou a regularidade real e descartou o ruído. Na prática estatística cotidiana, esse trade-off comparece em critérios como o **AIC** (Akaike, 1974) e o **BIC** (Schwarz, 1978), que medem o ajuste de um modelo e dele subtraem uma **penalidade proporcional ao número de parâmetros**. Mais botões para girar exigem pagar mais imposto.

Tudo isso confluí num único fenômeno que dá nome à seção seguinte: o **[[sobreajuste]]** (*overfitting*). Voltemos à curva. Com dez pontos no plano, um polinômio de grau nove passa por **todos** exatamente, resíduo zero — desempenho perfeito sobre os dados que já temos. Uma reta, ao contrário, erra um pouco em cada ponto. A tentação é coroar o polinômio. Mas peça aos dois que prevejam o **próximo** ponto, ainda não observado, e a reta humilha o polinômio: este, flexível demais, ajustou-se ao **ruído** de cada medição em vez da tendência por baixo dele, e por isso oscila grotescamente fora da amostra. Acrescentar parâmetros **sempre** melhora o ajuste interno e quase sempre piora a previsão externa a partir de certo ponto. A simplicidade, neste registro, não é gosto: é blindagem contra confundir ruído com sinal — o eixo do dilema **[[viés-variância]]**.

## Os limites

A primeira ilusão a quebrar é a mais comum: a navalha **não é um critério de verdade**. Nada na natureza promete ser simples. O genoma é barroco, a química do metabolismo é um labirinto, a física de partículas postula um zoológico de entidades que ninguém escolheria por elegância. A navalha governa **como apostar diante da ignorância**, não como o mundo está montado. Preferir o simples é racional como estratégia de inferência; supor que o mundo *é* simples porque a navalha o prefere inverte a flecha e comete um erro categorial.

A segunda fragilidade está na pré-condição. A igualdade de adequação explicativa, que liga o mecanismo, **quase nunca se realiza exatamente**. No mundo real, a hipótese mais complexa costuma ajustar-se um pouco melhor aos dados, e a mais simples um pouco pior. Não há então empate a desempatar: há uma **troca** entre quanto de ajuste se abre mão em nome de quanta parcimônia se ganha — e **não existe taxa de câmbio neutra** entre essas duas moedas. AIC e BIC propõem taxas específicas, e discordam entre si justamente porque a conversão é uma decisão, não uma dedução. A navalha aponta a direção; não fixa o preço.

A terceira fragilidade, a mais profunda, é a **relatividade da simplicidade à linguagem**, e Nelson Goodman a expôs com crueldade no enigma do *grue* (Goodman, 1955). Defina a propriedade *verzul*: aplica-se a algo verde se observado antes de certa data e azul se observado depois. A hipótese "todas as esmeraldas são verdes" parece simplíssima — mas só porque nosso vocabulário tem "verde" e não "verzul". Num idioma que tomasse *verzul* como primitivo, "todas as esmeraldas são verdes" seria a hipótese *complexa*, e "todas são verzuis", a simples. O que conta como **uma** suposição, como **uma** entidade, depende do vocabulário em que a descrevemos — e a navalha, sozinha, não escolhe o vocabulário. Ela herda sua autoridade do **conhecimento de fundo** que torna certos predicados naturais e outros artificiais; não a extrai da pura lógica.

Disso decorre a tese de Elliott Sober, a crítica filosófica mais madura ao tema: **não existe uma navalha, mas várias** (Sober, 2015). Em contextos diferentes — filogenia, seleção de modelos, metafísica — invocam-se princípios de parcimônia diferentes, e cada um precisa de **justificação local e empírica própria**, ancorada no que já se sabe sobre aquele domínio. Não há um princípio único, *a priori*, que valha em todo lugar por mérito puramente racional. A navalha é uma família de ferramentas, cada qual afiada para um material específico.

Há ainda o erro espelhado do excesso de zelo: a parcimônia levada longe demais vira **subajuste** (*underfitting*). Uma teoria simples demais ignora estrutura real e prevê tão mal quanto a complexa que persegue ruído. A virtude está num ponto intermediário, não no mínimo absoluto de suposições. Por fim, e talvez seja o abuso mais frequente fora dos laboratórios, a navalha é convertida em **cassetete retórico**: invoca-se "a explicação mais simples" para encerrar à força um debate cuja complexidade é genuína e está sustentada por evidência. Esse movimento não usa a navalha — usa o seu prestígio. É contra ele que a próxima seção arma a defesa.

## Na prática

No trabalho científico e estatístico, a navalha é rotina operacional sob outros nomes. Ao comparar modelos, prefere-se o de **menos parâmetros livres** quando o ganho de ajuste do modelo maior não compensa o imposto de complexidade que AIC, BIC ou a regularização cobram. Em aprendizado de máquina, técnicas de **regularização** existem literalmente para penalizar complexidade e conter o sobreajuste — a navalha codificada como termo na função de custo.

Na medicina diagnóstica, a parcimônia ganhou apelido próprio: a regra de preferir a **hipótese diagnóstica única** capaz de explicar todos os sintomas, em vez de empilhar vários males independentes. Mas o domínio também oferece o contrapeso mais elegante a qualquer parcimônia ingênua — o **dito de Hickam**: *um paciente pode ter tantas doenças quantas queira ter*. Em pacientes idosos ou cronicamente enfermos, a base estatística muda: várias condições coexistentes tornam-se **mais prováveis** que um único diagnóstico exótico que costure tudo. O dito não revoga a navalha; lembra que a parcimônia compete sempre com a probabilidade de base, e que diante de evidência basta de múltiplas causas, é a história simples que deve cair. Em depuração de software e em manutenção de equipamentos, a mesma sabedoria vira protocolo: antes da causa exótica, teste a banal — o cabo solto antes do *bug* no compilador.

O eixo de defesa cognitiva, porém, é o que mais importa para quem usa a navalha como escudo num debate. Ela é, com frequência, **virada contra a pessoa** por um interlocutor que anuncia "a explicação mais simples é a minha" e despacha o que o incomoda como complicação gratuita. Três verificações desmontam a manobra.

A primeira: **a explicação "simples" está mesmo dando conta de todos os fatos?** Quase sempre o atalho retórico só parece econômico porque **varreu evidência para baixo do tapete**. Restaure a evidência ignorada e o suposto empate evapora — sem empate, a navalha sequer se aplica, e a explicação que de fato cobre os dados vence, por mais elaborada que seja. A parcimônia jamais autoriza descartar evidência para manter a história arrumada.

A segunda: **em que vocabulário "simples" foi medido?** Como mostrou o enigma de Goodman, a simplicidade depende do enquadramento, e enquadramentos podem ser carregados de propósito. Pergunte se a economia alegada sobrevive a uma redescrição neutra do problema, ou se ela depende de um vocabulário escolhido justamente para fazer um lado parecer enxuto.

A terceira: **a navalha está sendo usada como desempate ou como trator?** Sua jurisdição legítima começa e termina nos empates explicativos. Quem a invoca para vencer apesar de ajustar pior os dados não a está aplicando — está sequestrando seu prestígio. A defesa cabe numa frase a ser dita em voz alta: *concordo em preferir o mais simples quando as explicações empatam; mostre-me primeiro que elas empatam*. Na ausência desse empate, a discussão volta para onde sempre deveria estar — a **evidência** —, e é ali, não na elegância, que se decide.

---
## Leitura recomendada

1. Brian Christian e Tom Griffiths. *Algoritmos para Viver.*
2. Carl Sagan. *O Mundo Assombrado pelos Demônios.*
3. Nate Silver. *O Sinal e o Ruído.*

## Referências

1. Akaike, Hirotugu. *A New Look at the Statistical Model Identification.* 1974.
2. Goodman, Nelson. *Fact, Fiction, and Forecast.* 1955.
3. Jefferys, William H.; Berger, James O. *Ockham's Razor and Bayesian Analysis.* 1992.
4. Kolmogorov, Andrei N. *Three Approaches to the Quantitative Definition of Information.* 1965.
5. MacKay, David J. C. *Information Theory, Inference, and Learning Algorithms.* 2003.
6. Ockham, Guilherme de. *Summa Logicae.* c. 1320.
7. Popper, Karl. *The Logic of Scientific Discovery.* 1959.
8. Rissanen, Jorma. *Modeling by Shortest Data Description.* 1978.
9. Schwarz, Gideon. *Estimating the Dimension of a Model.* 1978.
10. Sober, Elliott. *Ockham's Razors: A User's Manual.* 2015.


