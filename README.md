# lnpg-cap8-selecao
Discente: Léo Bernardo da Silva Santos

Atividade prática do Capítulo 8, Estruturas de Seleção

LLM usado: Grok.

q1_loops.md:

Análise: 

*Python*:
Quantidade de Linhas: 8, muito compacto; Legibilidade: Extremamente claro, qualquer pessoa que sabe programar o mínimo entende bem rápido. Sintaxe limpa, sem ruído. Concisão: Ganha de todos. É o rei da concisão sem sacrificar clareza na maioria dos casos.

*Swift*:
Quantidade de Linhas: 12, limpo e organizado; Legibilidade: Muito legível também. Parece Python mas com tipos,   as variáveis são bem naturais. Concisão: tão bom quanto Python, especialmente em scripts pequenos.

*Haskell*:
Quantidade de Linhas: 13, Legibilidade: Muito elegante se você entende recursão, mas para um iniciante ou programador comum, parece grego. Concisão:é conciso na lógica, mas o módulo e a assinatura de funções deixam ele parecido com os outros.

*Java*:
Quantidade de Linhas: 18, o que contem mais palavras. Legibilidade: Funciona, mas tem muito arrodeio (classe pública, public static void main, etc). O código de verdade fica perdido no meio. Concisão: é o mais pesado, dificultoso.

*Opinião pessoal*:
Python sempre me é uma primeira alternativa nessas situações. Parece que estou rabiscando um rascunho que ganha vida. A sintaxe some, você foca na solução e, ela se materializa. Chega a ser relaxante.
Programar em Swift é satisfatório. Transmite uma vibe de "inovador e confiável". Imagine Python depois de uma dose de café e um upgrade no visual. É minha escolha para apps e quando a agilidade e clareza são essenciais.
Java, lembra aquele parente conservador que não abre mão do formalismo nem na praia? É funcional, robusto, universalmente conhecido, mas denota a idade. Ideal para projetos extensos e vitais, mas para algo rápido? Exagero total.
Haskell é pura arte. Quando a lógica se revela, sua sofisticação me encanta. Mas, sejamos sinceros: em geral, penso "que primor... agora, por gentileza, repita, porque me passou batido da primeira vez".

Comparação:
Para quem nunca viu, Rust pode parecer ter uma clareza intermediária, algo entre Swift e Haskell. Mas, depois de pegar o jeito, a coisa muda completamente. Ele oferece a segurança de Haskell combinada com a praticidade que Swift entrega hoje em dia.

q2_selecao.md:

Análise:

*Ruby*:
Quantidade de linhas: 13. Legibilidade: Extremamente limpo e natural, parece até português. Concisão: Essa ganha, pois expressa a intenção com o mínimo de palavras.

*C*:
Quantidade de linhas: 23, muito verboso. Legibilidade: Clássico, a maioria entende, porém tem muito ruído. Concisão: último lugar, precisa de muito código cerimonial.

*Erlang*:
Quantidade de linhas: 19, meio termo. Legibilidade: A sintaxe com guards (when K =:= ...) é poderosa, mas estranha na primeira vista. Parece mais "matemática" que "programação comum". Concisão: É conciso na lógica, mas cheio de formalidades.

*Opinião pessoal*:

Ruby me traz felicidade. É como se a linguagem estivesse ao meu lado, colaborando. Seu estilo de escrita é, provavelmente, o mais elegante entre as linguagens convencionais. Programar em Ruby, para mim, é quase terapêutico — parece que estou descrevendo o que desejo, em vez de codificar.

C é como um velho amigo confiável, mas um tanto tedioso. Ele exige que tudo seja feito manualmente: incluir bibliotecas, declarar a função main, inserir break em cada case (sob risco do clássico bug), retornar 0... É seguro e rápido, mas carrega o peso dos anos 70. Funciona bem, mas não é prazeroso.

Erlang, por sua vez, me fascina e intimida ao mesmo tempo. A forma como utiliza pattern matching e guards é engenhosa e extremamente poderosa, especialmente para sistemas concorrentes. Contudo, sua sintaxe é bastante peculiar para quem vem de linguagens mais comuns. Parece que estamos escrevendo regras matemáticas, e não código. É uma linguagem que exige uma mudança completa de mentalidade.

Comparação:
Minha opinião sincera, comparando as quatro linguagens:
Ruby → É a mais prazerosa de escrever e ler quando se trata desse tipo de código.
Rust → Representa o equilíbrio ideal atualmente: segurança, elegância e desempenho.
C → É confiável, mas acaba sendo cansativo.
Erlang → Muito inteligente, mas sinto que preciso adaptar minha forma de pensar para usá-lo.

Se fosse resolver esse exercício rapidamente para testar lógica, escolheria Ruby.
Se fosse um projeto real e de maior responsabilidade, optaria por Rust.
Agora, se o contexto fosse sistemas de telefonia ou ambientes de alta concorrência, aí sim Erlang ou Elixir mostram todo o seu valor.

q3_sem_goto.md:

Análise: 

*Python*:
Quantidade de Linhas: 12. Concisão: Alta no contexto imperativo. Python remove chaves e parênteses desnecessários, resultando em um código enxuto. Legibilidade: Excelente para quem pensa sequencialmente. O uso de indentação semântica obriga o código a ser limpo visualmente. O fluxo de controle com if/elif/else é direto e fácil de seguir como uma "receita de bolo".

*Java*:
Quantidade de Linhas: 16. Concisão: Baixa. Java é conhecido por ser uma linguagem mais "verbosa". A necessidade de declarar o tipo primitivo (int), usar chaves {} para delimitar blocos e ponto e vírgula ; adiciona ruído visual. Legibilidade: Muito boa para equipes grandes ou para quem vem de linguagens com sintaxe estilo C. A estrutura em blocos deixa os limites do escopo extremamente explícitos, mas o excesso de caracteres não alfanuméricos polui um pouco a leitura da lógica central.

*Haskell*:
Quantidade de Linhas: 11 linhas operacionais (a mais curta). Concisão: Altíssima. O uso de Guards (|) condensa a lógica de ramificação de forma matemática e elegante. Legibilidade: Depende fortemente do seu background. Para programadores não familiarizados com o paradigma funcional, pode parecer alienígena no início, pois substitui o laço while por recursão e remove o conceito de variáveis mutáveis. No entanto, uma vez que você entende a sintaxe, a leitura é extremamente semântica: a lógica do nextJ lida com a atualização do estado de forma segura e livre de efeitos colaterais.

*Opinião pessoal*:
O Código Haskell é o mais elegante e seguro. A ausência de estado mutável (não reatribuir valor a i e j durante o loop) previne uma classe inteira de bugs conhecidos como "side-effects" (efeitos colaterais). Ele obriga você a descrever o que é o resultado, e não como alterar a memória passo a passo.
Python é o mais pragmático. Para um script rápido, análise de dados ou automação, é difícil bater a velocidade de leitura e escrita do Python.
Java é o "arroz com feijão" da indústria. Apesar de verboso, a tipagem estática e a estrutura rígida são o motivo pelo qual ele é a espinha dorsal de sistemas corporativos complexos.

q4_for_multilinguagens.md

Análise:

*C*:
Quantidade de Linhas: 10. Concisão: Altíssima no controle de fluxo. É a única do seu grupo original que permite inicializar, verificar e incrementar múltiplas variáveis (i e j) na mesma declaração do for. Legibilidade: Direta e mecânica. Todo o gerenciamento de estado do loop fica concentrado em uma única linha, separando claramente o que é "controle" do que é "lógica de negócio" (o cálculo de sum).

*Python*:
Quantidade de Linhas: 11. Concisão: Baixa neste cenário específico. Como o for do Python é exclusivamente um foreach projetado para iterar sobre coleções ou ranges (e não suporta múltiplas variáveis de controle nativamente sem o uso avançado de zip ou itertools), o uso do while torna o código mais longo e manual. Legibilidade: Clara, mas suscetível a erros. O desenvolvedor precisa lembrar de incrementar i e decrementar j no final do bloco, o que em loops maiores pode gerar bugs (loop infinito).

*Kotlin, Rust e Swift*:
Quantidade de Linhas: ~11 a 13. Concisão: Média. Todas elas abandonaram o for clássico do C em favor da iteração sobre Ranges (0 until n, 0..n, 0..<n). Isso torna o controle da variável principal (i) muito limpo, mas obriga a variável secundária (j) a ser declarada fora e mutada manualmente dentro do bloco. Legibilidade: Excelente. A sintaxe de range é extremamente semântica e fácil de ler (lê-se como "para i de 0 até n"). O fato de declararem tipos de forma explícita ou por inferência forte (como o let mut no Rust) deixa a intenção do programador óbvia e segura.


*Opinião Pessoal*:
A evolução do for clássico (C) para os iteradores baseados em ranges (Rust, Kotlin, Swift) reflete uma mudança de prioridade na engenharia de software: focar mais na segurança do que na flexibilidade extrema.
O Vencedor Técnico (Neste cenário): C e Go. Se o seu problema central exige a manipulação paralela e síncrona de múltiplos contadores, o for clássico é imbatível. Ele previne que você esqueça de atualizar a segunda variável, pois a atualização fica no cabeçalho do laço.
Kotlin/Rust/Swift. Embora exijam que j seja gerenciado manualmente neste exemplo específico, em 95% do desenvolvimento moderno nós iteramos sobre coleções (listas, arrays), e não gerenciando ponteiros matemáticos numéricos. Os ranges evitam os clássicos bugs de "off-by-one" (errar por um dígito, como usar <= em vez de <).
Python: É a menos elegante para este problema específico. Python brilha quando o código é "Pythônico" (ex: sum(i * j + 3 for i, j in zip(range(n), range(17, 17-n, -1)))), mas tentar escrever código imperativo puro nela geralmente resulta em soluções verbosas.
