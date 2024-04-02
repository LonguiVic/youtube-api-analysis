
# Youtube API Analysis

Este script em Python foi desenvolvido para extrair dados estatísticos e de conteúdo do YouTube usando a API do YouTube Data API v3. Ele fornece insights sobre canais do YouTube, vídeos individuais e comentários associados aos vídeos.


## Referência

 - [The Vu data analytics](https://www.youtube.com/watch?v=D56_Cx36oGY)

## Apêndice

Coloque qualquer informação adicional aqui


## Autores

- [@LonguiVic](https://github.com/LonguiVic)


## Instalação

- Python 3.x
```bash
  https://www.python.org/downloads/release/python-3810/
```

- seaborn

```bash
  pip install seaborn
```
- matplotlib
```bash
  pip install matplotlib
```
- nltk
```bash
  pip install nltk
```
- wordcloud
```bash
  pip install wordcloud
```
- pandas
```bash
  pip install pandas
```
- jupyter
```bash
  pip install jupyter
```
- google-api-python-client
```bash
  pip install google-api-python-client
```


## Documentação

[Seaborn](https://seaborn.pydata.org/installing.html)

[Matplotlib](https://matplotlib.org/stable/index.html)

[Youtube API v3](https://console.cloud.google.com/apis/library/youtube.googleapis.com?project=new-project-418921)

[Pandas](https://pandas.pydata.org/docs/)

[dateutil](https://pypi.org/project/python-dateutil/)

[nltk](https://www.nltk.org)

## Como Usar o Script

### Configuração da API do youtube
- É necessário obter uma chave de API do YouTube. Essa chave deve ser inserida na variável *api_key* no script.

### Especificar IDs dos Canais
- Defina os IDs dos canais que deseja analisar na lista *channel_ids.*

### Execução do Script
- Execute o script em um ambiente Python. Certifique-se de que todas as bibliotecas necessárias estejam instaladas.
- Também é possível executar pelo jupyter, caso prefira.

### Visualização dos Resultados
- O script fornecerá diversas visualizações e insights sobre os canais, vídeos e comentários extraídos.

## Funções Principais do Script

### _get_channel_stats(youtube, channel_ids)_
- Esta função obtém estatísticas dos canais especificados, como número de inscritos, visualizações totais e total de vídeos. Retorna um DataFrame Pandas com essas informações.

### _get_video_ids(youtube, playlist_id)_
- Esta função obtém os IDs de vídeo de uma lista de reprodução específica. Retorna uma lista de IDs de vídeo.

### _get_video_details(youtube, video_ids)_
- Esta função obtém detalhes de vídeos específicos, como título, descrição, contagem de visualizações e contagem de comentários. Retorna um DataFrame Pandas com essas informações.

### _get_comments_in_videos(youtube, video_ids)_
- Esta função obtém os principais comentários de vídeos específicos. Devido às limitações da API do YouTube, apenas os primeiros 10 comentários são extraídos para cada vídeo. Retorna um DataFrame Pandas com os IDs de vídeo e os comentários associados.

## Análises Realizadas
- Vídeos com melhor desempenho
- Vídeos com pior desempenho
- Distribuição de visualização por vídeo
- Visualização VS Likes e comentários
- Duração dos vídeos
- Programação de uploads
- Nuvem de palavras geradas a partir dos títulos dos vídeos para identificar os termos mais comuns

## Considerações
- Este script foi desenvolvido com base na versão 3 da API do YouTube. Qualquer atualização subsequente na API pode exigir modificações no script.
- Certifique-se de seguir as políticas de uso da API do YouTube ao utilizar este script em produção, especialmente em relação às cotas de uso da API.

## Conclusão
Este script fornece uma maneira eficiente de extrair e analisar dados do YouTube, permitindo insights valiosos sobre o desempenho de canais, vídeos individuais e interações de comentários. É útil para criadores de conteúdo, profissionais de marketing digital e pesquisadores interessados em entender melhor o ecossistema do YouTube.




