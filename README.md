# AI_900_TEXT_ANALYSIS

## Analisar texto com o Language Studio

Neste exercício, você explorará as capacidades do Azure AI Language analisando algumas avaliações de hotéis como exemplo. Você usará o Language Studio para entender se as avaliações são principalmente positivas ou negativas.

O Processamento de Linguagem Natural (NLP) é um ramo da IA que lida com linguagem escrita e falada. Você pode usar NLP para construir soluções que extraem significado semântico de texto ou fala, ou que formulam respostas significativas em linguagem natural.

Por exemplo, suponha que a agência de viagens fictícia Margie’s Travel incentive os clientes a enviar avaliações para estadias em hotéis. Você poderia usar o serviço de Linguagem para identificar frases-chave, determinar quais avaliações são positivas e quais são negativas, ou analisar o texto da avaliação em busca de menções a entidades conhecidas, como locais ou pessoas.

O Azure AI Language Service inclui capacidades de análise de texto e NLP. Estas incluem a identificação de frases-chave no texto e a classificação do texto com base no sentimento.

### Criar um recurso de Linguagem

Você pode usar muitos recursos de Linguagem do Azure AI com um recurso de Linguagem ou de serviços Azure AI. Existem algumas instâncias em que apenas um recurso de Linguagem pode ser usado. Para o exercício abaixo, usaremos um recurso de Linguagem. Se você ainda não o fez, crie um recurso de Linguagem em sua assinatura do Azure.

Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com, faça login com a conta da Microsoft associada à sua assinatura do Azure.

Clique no botão ＋ Criar um recurso e pesquise por serviço de Linguagem. Selecione criar um plano de serviço de Linguagem. Você será levado a uma página para selecionar recursos adicionais. Mantenha a seleção padrão e clique em Continuar para criar seu recurso.

Na página Criar Linguagem, configure-o com as seguintes configurações:

- Assinatura: Sua assinatura do Azure.
- Grupo de recursos: Selecione ou crie um grupo de recursos com um nome único.
- Região: East US.
- Nome: Insira um nome único.
- Nível de preços: Free F0 ou S se Free F0 não estiver disponível.
- Ao marcar esta caixa, reconheço que li e entendi todos os termos abaixo: Selecionado.
  Selecione Revisar + criar e depois Criar e aguarde o término da implantação.

## Configurar seu recurso no Azure AI Language Studio

Em outra aba do navegador, abra o Language Studio em [https://language.cognitive.azure.com](https://language.cognitive.azure.com) e faça login.

Quando solicitado a selecionar um recurso do Azure, faça as seguintes configurações:

- Diretório do Azure: Diretório Padrão, o diretório que você está usando
- Assinatura do Azure: Selecione a assinatura que você está usando
- Tipo de recurso: Linguagem
- Nome do recurso: selecione o recurso de serviço de Linguagem que você acabou de criar
  Em seguida, selecione Concluído.

## Analisar avaliações no Language Studio

Em um navegador da web, acesse o Language Studio em [https://language.cognitive.azure.com](https://language.cognitive.azure.com).

Na página inicial do Bem-vindo ao Language Studio, selecione a aba Classificar texto e, em seguida, selecione o bloco Analisar sentimento e minerar opiniões.

Em Selecionar idioma do texto, selecione Inglês.

Em Selecionar seu recurso do Azure, selecione seu recurso.

Em Digite seu próprio texto, faça upload de um arquivo ou use um de nossos textos de amostra, copie e cole a seguinte avaliação:

````json
 Tired hotel with poor service
 The Royal Hotel, London, United Kingdom
 5/6/2018
 This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.```
````
