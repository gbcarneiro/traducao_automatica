# traducao_automatica

**1. Tente valores diferentes do argumento num_examples na funçãoload_data_nmt. Como isso afeta os tamanhos do vocabulário do idioma de origem e do idioma de destino?**

À medida que aumentamos o número de exemplos (`num_examples`), os vocabulários dos idiomas de origem (inglês) e de destino (francês) também aumentam. Com poucos exemplos, o vocabulário é pequeno, contendo apenas algumas palavras e expressões. Conforme o número de exemplos cresce, o vocabulário se expande, capturando uma maior quantidade de palavras, variações e expressões, o que torna o modelo mais eficaz.

**2. O texto em alguns idiomas, como chinês e japonês, não tem indicadores de limite de palavras (por exemplo, espaço). A tokenização em nível de palavra ainda é uma boa ideia para esses casos? Por que ou por que não?**

Para idiomas como chinês e japonês, a tokenização em nível de palavras não é ideal devido à falta de delimitadores e à ambiguidade na segmentação. Abordagens em nível de caracteres ou subpalavras são mais apropriadas, pois capturam a estrutura e o significado do texto de forma mais eficiente.