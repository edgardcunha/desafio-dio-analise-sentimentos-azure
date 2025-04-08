# Análise de Sentimentos com Language Studio no Azure AI (Desafio DIO)

Este repositório documenta a realização do desafio da DIO sobre "Análise de Sentimentos utilizando o Azure AI Language Studio". O objetivo foi explorar a ferramenta da Microsoft Azure para analisar um conjunto de frases e extrair insights sobre o sentimento expresso nelas.

## 🚀 Ferramentas Utilizadas

*   **Azure AI Language Studio:** Plataforma online da Microsoft Azure para experimentar e utilizar serviços de IA de Linguagem.
*   **GitHub:** Para versionamento e documentação do projeto.

## 📝 Processo Realizado

1.  **Criação das Sentenças de Entrada:** Foi criado um arquivo de texto (`inputs/sentences.txt`) contendo diversas frases (simulando avaliações de um produto fictício) com diferentes cargas de sentimento (positivas, negativas, neutras e mistas).
    *   [Link para o arquivo de entrada](./inputs/sentences.txt)
2.  **Acesso ao Azure AI Language Studio:** Acessei o portal do [Azure AI Language Studio](https://language.cognitive.azure.com/).
3.  **Seleção do Recurso:** Dentro do Language Studio, selecionei a funcionalidade "Analyze sentiment and mine opinions".
4.  **Configuração da Análise:**
    *   Escolhi a opção de inserir o texto diretamente.
    *   Selecionei o idioma do texto (Português - Brasil).
    *   Colei o conteúdo do arquivo `sentences.txt` na área de texto.
    *   Executei a análise clicando em "Run".
5.  **Observação dos Resultados:** A ferramenta processou as sentenças e apresentou:
    *   Um sentimento geral para todo o texto.
    *   O sentimento individual para cada sentença (Positivo, Negativo, Neutro ou Misto).
    *   Scores de confiança para cada classificação de sentimento (indicando a "certeza" da IA).
    *   Mineração de Opinião: Identificação de *targets* (assuntos, como "bateria", "design") e *assessments* (opiniões sobre esses assuntos, como "dura pouco", "bonito").

## 📊 Resultados e Prints

A análise no Language Studio identificou corretamente a polaridade da maioria das frases.

`![Resultado da Análise no Language Studio](link_para_sua_imagem.png)`

**Resultado:**
A ferramenta atribuiu um sentimento geral **Misto** ao conjunto de textos, refletindo a variedade de opiniões. Frases como "Amei a caneca inteligente!" foram classificadas como **Positivas** com alta confiança, enquanto "Que decepção. A bateria dura muito pouco..." foi classificada como **Negativa**. A frase "A ideia da caneca é ótima [...] mas a conexão Bluetooth falha..." foi corretamente identificada como **Mista**.

## ✨ Insights e Aprendizados

*   **Granularidade:** O Language Studio permite analisar tanto o sentimento geral de um bloco de texto quanto o sentimento específico de cada sentença, o que é muito útil para entender nuances.
*   **Confiança:** Os scores de confiança ajudam a avaliar a assertividade da análise da IA. Scores mais baixos podem indicar frases mais ambíguas ou complexas.
*   **Sentimento Misto:** A capacidade de detectar sentimentos mistos em uma única frase é um recurso poderoso, pois reflete como as pessoas frequentemente expressam opiniões (elogiando um aspecto e criticando outro).
*   **Mineração de Opinião (Opinion Mining):** A funcionalidade adicional de identificar *o que* está sendo elogiado ou criticado (aspectos/targets) leva a análise a um nível mais profundo, permitindo entender *por que* o sentimento é positivo ou negativo.
*   **Facilidade de Uso:** O Language Studio oferece uma interface intuitiva que permite testar e visualizar rapidamente as capacidades dos serviços de IA de Linguagem do Azure sem precisar escrever código inicialmente.

## 🔮 Possibilidades

A análise de sentimentos com ferramentas como o Azure AI Language Studio abre diversas possibilidades:

*   **Monitoramento de Marca:** Analisar menções em redes sociais e notícias para entender a percepção pública.
*   **Feedback de Clientes:** Processar automaticamente avaliações de produtos, pesquisas de satisfação e tickets de suporte para identificar pontos fortes e fracos.
*   **Pesquisa de Mercado:** Avaliar a recepção de novos produtos ou campanhas.
*   **Análise de Funcionários:** Entender o sentimento em pesquisas internas de clima organizacional (com devida atenção à privacidade e ética).
*   **Moderação de Conteúdo:** Identificar automaticamente conteúdo potencialmente tóxico ou abusivo em plataformas online.

## 🔗 Links Úteis

*   [Explore o Azure AI Language Studio](https://language.cognitive.azure.com/)
*   [Documentação: Analyze text with Language Studio](https://learn.microsoft.com/en-us/azure/ai-services/language-service/language-studio)