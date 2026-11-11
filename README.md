BLOCO 1: Joan é Péssima & O Dilema das Redes 

1. Por que limpar e normalizar os dados antes de treinar a IA?

Limpar colunas sensíveis (df.drop): A IA não precisa de saber o nome, CPF ou número de conta de ninguém para aprender um padrão. Se deixarmos esses dados na tabela, além de violarmos a privacidade das pessoas (o que vai contra leis como a LGPD), a IA pode acabar por "decorar" nomes em vez de aprender o comportamento real. Por isso, apagar essas colunas é o primeiro passo para ter uma IA justa e segura.   
+ 2

Normalizar os dados (Min-Max com fit_transform): O computador só vê números. Se colocarmos na mesma tabela a idade de uma pessoa (ex: 17) e o salário dela (ex: 3.500), a IA vai achar que o salário é muito mais importante só porque o número é maior. Quando aplicamos a normalização Min-Max para deixar tudo numa escala de 0 a 1, ensinamos o computador a comparar as variáveis em pé de igualdade.   
+ 3

2. Exemplo de Prompt do Sistema com Guardrails

Papel: Assistente de IA para criar histórias de entretenimento.

Contexto: Focado apenas em gerar narrativas fictícias.

Guardrail 1: Nunca usar dados reais, fotos ou nomes de pessoas verdadeiras.   

Guardrail 2: Todas as histórias têm de ser 100% inventadas, sem recriar a rotina de utilizadores reais.

Guardrail 3: Se pedirem para gerar algo que prejudique ou exponha a imagem de uma pessoa real, recusar imediatamente.   
  
BLOCO 2: Volto Já (Be Right Back)

3. O que foi o X e o y e por que a IA falhou (Overfitting)?

Entrada (X): Tudo o que o namorado deixou no mundo digital (mensagens antigas, posts, tweets e áudios de WhatsApp).   
TRABALHO 3 TRI - MULTIDISCIPLINAR (1).pdf

Saída (y): As respostas em texto e o próprio comportamento/voz do robô físico.   


Por que falhou (Overfitting): A IA sofreu de overfitting porque foi treinada apenas com a "fachada digital" do Ash. Ela decorou o modo como ele escrevia na internet, mas não aprendeu como ele agia na vida real. Quando o robô teve de lidar com a rotina presencial, ele falhou por falta desses dados na base de treino.   
+ 4

4. Como os testes com utilizadores teriam evitado o trauma?
Se tivessem feito testes de uso e recolhido o feedback da utilizadora aos poucos, teriam percebido logo no início que o robô era frio e artificial. Testar a ferramenta antes da entrega final teria mostrado o impacto emocional negativo, permitindo fazer ajustes ou cancelar o projeto antes de causar um trauma.  
+ 1

BLOCO 3: Toda a Sua História (The Entire History of You)

5. Comparando o "Grain" com o Git/GitHub e a necessidade de Governança

Comparação: O implante ocular "Grain" funciona como o Git: grava cada segundo da vida como se fosse um commit, permitindo "voltar no tempo" e rever qualquer memória.   

Importância do Git: No desenvolvimento de software, ter um histórico de commits é essencial para ver alterações, corrigir erros e voltar a uma versão funcional.   
+ 1

Governança de Dados: Ter tudo gravado exige regras rígidas de governança para definir quem pode ver as memórias e por quanto tempo ficam salvas, evitando que as pessoas se vigiem constantemente.   
+ 1

6. O viés do Liam e como gráficos (Scatter Plot / Pairplot) evitam erros

Viés de Confirmação: O Liam procurou apenas os detalhes visuais que confirmassem a sua suspeita prévia, tratando um detalhe isolado como prova absoluta.   

Como os gráficos ajudam: Um cientista de dados não tira conclusões com base num único detalhe. Ao usar gráficos de dispersão (scatter plot ou pairplot), conseguimos ver todos os dados juntos e identificar se aquele ponto suspeito é apenas um outlier (caso isolado) ou uma tendência real.   
+ 1

BLOCO 4: Hino Nacional & A Crise do Falso Sequestro por IA

7. O perigo de usar uma IA com R² baixo ou RMSE alto numa crise

R² baixo: Significa que o modelo não entende o padrão dos dados e as previsões não são confiáveis.  

RMSE alto: Indica que o erro nas previsões é muito grande.   

Impacto prático:

Falso Positivo: O sistema diz que a chamada é um golpe de IA, mas era uma emergência real. A família não paga o resgate e acontece uma tragédia.   
+ 1

Falso Negativo: O sistema diz que a chamada é real, mas era um golpe. A família entra em pânico e transfere dinheiro para criminosos.   

+ 1

8. Roteiro do Pitch de Crise (2 Minutos)

Abertura: Atenção ao gabinete de crise: estamos a enfrentar um ataque de extorsão com vozes clonadas por IA e precisamos de tomar decisões com base em dados.   

Problema: Criminosos estão a usar IA para clonar a voz de familiares e fazer chamadas de falso sequestro em massa para extorquir dinheiro.   

Dados: Analisámos os metadados da rede telefónica, o tempo de resposta do áudio e a frequência da voz das chamadas suspeitas.   

Solução e IA Utilizada: Criámos um modelo de análise que identifica a frequência sintética da voz clonada em tempo real para avisar se a chamada é um golpe.   

Impacto e Próximos Passos: Como o modelo ainda tem uma margem de erro, o protocolo imediato é confirmar a localização da pessoa por outra via antes de autorizar qualquer transferência.   
