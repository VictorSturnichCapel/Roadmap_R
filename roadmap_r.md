
1. Introdução às Expressões Regulares
O que são expressões regulares?
Entenda que são padrões usados para encontrar e manipular texto. São uma ferramenta poderosa para análise de dados.

Casos de uso em Ciência de Dados:

Limpeza de dados (remoção de espaços, pontuações, etc.)

Extração de informações específicas (como e-mails, números de telefone)

Verificação de padrões em dados (como padrões em strings de texto)

2. Fundamentos das Expressões Regulares
Metacaracteres Básicos:

. (ponto) – Corresponde a qualquer caractere, exceto nova linha.

^ – Início da string.

$ – Fim da string.

[] – Definem um conjunto de caracteres.

| – Alternância (ou).

() – Agrupamento de subexpressões.

Quantificadores:

* – 0 ou mais vezes.

+ – 1 ou mais vezes.

? – 0 ou 1 vez.

{n} – Exatamente n vezes.

{n,} – Pelo menos n vezes.

{n,m} – Entre n e m vezes.

Exemplos práticos:

Encontrar palavras que começam com uma letra maiúscula: ^[A-Z]

Encontrar números de telefone: \(\d{2}\) \d{4,5}-\d{4}

3. Operadores Avançados e Funções
Caractere de Escape:

\ – Para escapar caracteres especiais como \. (ponto literal) ou \* (asterisco literal).

Classes de Caracteres:

\d – Qualquer dígito (0-9).

\D – Qualquer caractere que não seja dígito.

\w – Qualquer caractere alfanumérico (letras e números).

\W – Qualquer caractere não alfanumérico.

\s – Qualquer caractere de espaço em branco.

\S – Qualquer caractere que não seja um espaço em branco.

4. Aplicações Práticas em Ciência de Dados
Limpeza de Dados:

Remover espaços em branco extras:
Regex: \s+

Remover caracteres indesejados de um texto:
Regex: [^a-zA-Z0-9]

Substituir partes específicas de uma string:
Exemplo: re.sub(r'\d+', 'NUMBER', 'abc 123')

Extração de Informações de Strings:

Extrair e-mails:
Regex: \b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b

Extrair URLs:
Regex: https?://(?:www\.)?[a-zA-Z0-9-]+\.[a-zA-Z]{2,6}(/[-a-zA-Z0-9@:%._\+~#=]*)?

5. Ferramentas e Bibliotecas para Trabalhar com Regex
Python:

re (biblioteca padrão do Python para regex)

Funções principais:

re.match(), re.search(), re.findall(), re.sub()

Jupyter Notebooks:
Testar e validar expressões regulares de forma interativa.

Online Regex Testing Tools:
Ferramentas como regex101 para testar e entender como suas expressões regulares funcionam.

6. Desafios e Melhoria de Habilidades
Prática de Casos Reais:

Encontre e limpe dados em conjuntos de dados desordenados.

Extraia informações específicas de textos ou relatórios.

Refine Expressões Regulares Complexas:

Crie regex para padrões mais complicados (como extrair tabelas de HTML, validar códigos postais, etc.).

7. Boas Práticas
Legibilidade:

Evite regexes muito complexos ou difíceis de entender. Use comentários sempre que necessário.

Desempenho:

Para grandes volumes de dados, preste atenção no desempenho das suas expressões regulares.

8. Avançando no Estudo
Regex em Big Data:

Como aplicar regex em ferramentas como Apache Spark ou Pandas para limpar grandes volumes de dados.

Regex para Machine Learning:

Use regex para extração de características de textos para modelos de NLP (Processamento de Linguagem Natural).

