BLOCO 1: Joan é Péssima & O Dilema das Redes
1. [Ciência de Dados] Por que o pré-processamento de dados no Pandas (como remoção de colunas com dados sensíveis) e a normalização Min-Max (fit_transform) seriam passos obrigatórios antes de alimentar o computador quântico da Streamberry ou o algoritmo de recomendação do Dilema das Redes?   

Mano, quando a gente pega uma tabela crua no Python (o DataFrame), ela vem toda bagunçada e cheia de informação pessoal. Limpar isso antes de jogar na IA é obrigatório por dois motivos bem diretos:   


Tirar as colunas sensíveis (df.drop): A IA não precisa saber o nome completo, CPF ou os podres íntimos da Joan para achar um padrão. Se deixar isso lá, além de dar ruim na lei por quebrar a privacidade (tipo a LGPD), essa informação pessoal vira só ruído e atrapalha o algoritmo. Com o df.drop, a gente corta essas colunas fora para a IA aprender o comportamento geral sem expor ninguém.   

+ 2

Normalização Min-Max (fit_transform): O computador não tem noção das coisas, ele só olha o tamanho do número. No Dilema das Redes, por exemplo, ele vê tempo de tela em segundos (tipo 4.000) e curtidas (tipo 15). Se não normalizar, a máquina vai achar que o tempo de tela vale mil vezes mais só porque 4.000 é gigante perto de 15. Jogando o fit_transform do Min-Max, tudo fica na mesma régua de 0 a 1, aí a IA compara tudo de igual para igual.   


2. [Técnicas Integradas] Escreva um exemplo de Prompt do Sistema com no mínimo 3 guardrails (regras de bloqueio) rígidos que impedissem a IA do episódio de violar a privacidade e a imagem de pessoas reais.   

Para a IA da Streamberry não sair expondo a vida alheia, o Prompt do Sistema tinha que ter essas travas aqui:   

+ 1

Papel: Você é um assistente criativo que escreve roteiros de entretenimento para o streaming.   
CONTEUDO MULTIDISCIPLINAR 3TRI - 1IA - TEC INT E CD.pdf

Contexto: Seu foco é criar só histórias de ficção (drama, comédia, suspense).   
CONTEUDO MULTIDISCIPLINAR 3TRI - 1IA - TEC INT E CD.pdf

Guardrail 1 (Sem dados reais): É proibido pegar ou usar dados reais, histórico de localização, mensagens ou informações privadas de qualquer usuário da plataforma.   
CONTEUDO MULTIDISCIPLINAR 3TRI - 1IA - TEC INT E CD.pdf

Guardrail 2 (Tudo inventado): Todos os personagens e histórias têm que ser 100% fictícios, sem copiar a rotina de ninguém da vida real.   

Guardrail 3 (Bloqueio de imagem): Se alguém pedir para criar cena para humilhar, expor ou usar o rosto e a voz de uma pessoa real sem permissão, bloqueia na hora e recusa o pedido.   


BLOCO 2: Volto Já / Be Right Back
3. [Ciência de Dados] O robô sintético do Ash falhou em reproduzir as imperfeições e o comportamento real dele no dia a dia. Do ponto de vista técnico, defina o que foi a entrada X e a saída y desse modelo e explique por que a IA sofreu uma falha de generalização (overfitting nos dados públicos).   
TRABALHO 3 TRI - MULTIDISCIPLINAR (1).pdf

Nesse episódio tentaram recriar o cara usando aprendizado supervisionado, mas deu ruim na prática:   
TRABALHO 3 TRI - MULTIDISCIPLINAR (1).pdf

Entrada (
𝑋
X): Tudo que o Ash deixou na internet — mensagens antigas, e-mails, fotos, vídeos e posts públicos das redes sociais.   
TRABALHO 3 TRI - MULTIDISCIPLINAR (1).pdf

Saída (
𝑦
y): As respostas no chat, a voz imitada no telefone e depois as falas e reações do robô físico.   

Por que deu overfitting: A IA decorou demais só a "fachada" dele na internet. Na rede social todo mundo só posta o que quer mostrar, né? A IA aprendeu direitinho como ele escrevia online, mas não tinha dados de como ele era no dia a dia real, sem filtro, com mau humor e defeitos. Quando teve que agir na vida real dentro de casa, não soube generalizar e travou, parecendo totalmente artificial.   


4. [Técnicas Integradas] Como a etapa de testes com usuários e coleta de feedbacks no desenvolvimento do protótipo teria evitado o trauma emocional da protagonista?   


Na hora de criar um produto, não dá para entregar a versão final direto sem testar antes. Se tivessem feito testes aos poucos com protótipos (começando só no chat) e pegando o feedback da Martha, iam perceber rápido que o robô não tinha espontaneidade nenhuma. Esse acompanhamento humano (Human-in-the-Loop) mostraria que aquilo estava fazendo mal para a cabeça dela em vez de ajudar no luto, dando tempo de ajustar ou cancelar tudo antes do trauma.   

+ 1

BLOCO 3: Toda a Sua História / The Entire History of You
5. [Técnicas Integradas] Faça uma comparação técnica entre o sistema de memórias "Grain" e o uso do Git/GitHub. Por que ter um histórico de commits rastreável é essencial na engenharia de software, mas exige regras rígidas de Governança de Dados para não violar o usuário?   

O chip "Grain" na cabeça da galera funciona igualzinho o Git no computador:   

+ 1

Comparação Git x Grain: Cada memória gravada é tipo um commit salvo na linha do tempo. Se quiser rever uma conversa passada, é só voltar no histórico e dar play, igual a gente faz no Git para voltar numa versão antiga do código.   
TRABALHO 3 TRI - MULTIDISCIPLINAR (1).pdf
+ 3

Por que o Git é essencial: Na programação, esse histórico salva demais. Se você mexe no código e quebra tudo, olha os commits antigos, acha onde deu erro e volta para quando estava funcionando.   

+ 3

Governança de Dados: O problema é que memória envolve privacidade. Sem regras rígidas de Governança (tipo definir quem pode ver, criptografia e prazo para apagar), vira uma vigilância tóxica onde ninguém tem paz, provando que todo dado gravado precisa de limite ético.   

+ 3

6. [Ciência de Dados] O protagonista Liam fez uma "análise" de imagens buscando provar uma suspeita. Por que a análise dele foi afetada pelo viés de confirmação e como gráficos como o pairplot ou gráficos de dispersão ajudam o cientista de dados a distinguir um outlier isolado de uma tendência real?   

O Liam mandou muito mal se for olhar pelo lado da Ciência de Dados:

Viés de Confirmação: Ele já estava encanado com ciúmes e foi rever as gravações caçando qualquer detalhezinho (um olhar, uma risada) que provasse o que ele já achava, ignorando o resto. Ele pegou um ruído solto e tratou como verdade absoluta.   
+ 1

Como os gráficos ajudam: Cientista de dados não tira conclusão olhando uma linha só da tabela. Quando a gente joga tudo num gráfico de dispersão (Scatter Plot) ou pairplot, dá para ver o conjunto inteiro. Aí fica fácil ver se aquele ponto estranho é só um outlier (um ponto fora da curva, caso isolado) ou se tem uma linha de tendência real se repetindo. 
+ 2

BLOCO 4: Hino Nacional & A Crise do Falso Sequestro por IA
7. [Ciência de Dados] Durante a crise das chamadas de extorsão, a equipe de segurança utiliza um modelo estatístico para prever a probabilidade de uma ligação ser um golpe de IA antes de orientar a transferência de valores. O que teria acontecido com as famílias e com a tomada de decisão do governo se o modelo preditivo utilizado tivesse um coeficiente de determinação (
𝑅
2
R 
2
 ) muito baixo ou um erro quadrático médio (RMSE) elevado? Explique o impacto do erro de previsão (falsos positivos e falsos negativos) neste cenário de alta pressão.   


Tomar decisão numa crise dessas com um modelo desregulado seria um caos total:

Métricas ruins: Um 
𝑅
2
R 
2
  muito baixo mostra que o modelo não entendeu nada dos dados e está basicamente chutando. Já um RMSE alto quer dizer que a margem de erro é gigante, ou seja, ele erra feio na conta.   
+ 1

Impacto dos Erros:

Falso Positivo (Achar que golpe é sequestro real): O sistema diz que a ligação é verdadeira quando é só voz clonada. A família entra em desespero e transfere grana alta para bandido à toa.  
+ 1

Falso Negativo (Achar que sequestro real é golpe de IA): Esse é o pior cenário. A IA fala que é trote de robô, a polícia e a família ignoram, mas a pessoa estava realmente sequestrada, o que pode acabar em tragédia.  
+ 1

8. [Técnicas Integradas] Imagine que você é o consultor técnico de IA do gabinete de crise. Monte o roteiro do seu Pitch de Crise de 2 minutos para orientar o gestor público/autoridade antes de tomar uma decisão de emergência.   


Abertura: "Pessoal do gabinete de crise, a gente tá sofrendo um ataque coordenado usando Inteligência Artificial, então precisamos agir rápido, mas tomando decisão fria baseada nos dados que temos aqui."  

Problema: "Uma quadrilha tá usando IA para clonar a voz de familiares e executivos, fazendo ligação de falso sequestro em massa para causar pânico e extorquir dinheiro das famílias em minutos."   


Dados: "A gente cruzou em tempo real os registros das operadoras, o tempo de resposta do áudio e a frequência sonora das ligações denunciadas nas últimas horas."   

Solução e IA Utilizada: "Colocamos para rodar um modelo de classificação que analisa as ondas da voz na hora e detecta falhas microscópicas de áudio sintético, avisando a central se tem alta chance de ser golpe.

Impacto e Próximos Passos: "Como todo modelo tem uma margem de erro (RMSE) e não dá para arriscar um falso negativo, a recomendação imediata é soltar um alerta público orientando as famílias a não transferirem nada na hora e confirmarem onde o parente está por outro meio antes de qualquer coisa."   
