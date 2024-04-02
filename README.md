
# Youtube API Analysis

Este script em Python foi desenvolvido para extrair dados estatísticos e de conteúdo do YouTube usando a API do YouTube Data API v3. Ele fornece insights sobre canais do YouTube, vídeos individuais e comentários associados aos vídeos.


## Referência

 - [The Vu data analytics](https://www.youtube.com/watch?v=D56_Cx36oGY)


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
### Vídeos com melhor desempenho
![best-performing](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/dc0be1f1-a033-4dd6-8cb6-60e4c3390a6a)
### Vídeos com pior desempenho
![worst](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/59a5146d-dd8c-4738-9b5a-de9658717fa5)
### Distribuição de visualização por vídeo
![view-dist](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/a785fe8d-7126-42c9-9c80-d0a7c58c2c9a)
### Visualização VS Likes e comentários
![view-vs-likes](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/6af656c9-3404-43ed-8c7e-db44d4003b6e)
### Duração dos vídeos
![image](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/2aaf696e-7c6e-4f9c-8f85-048b80e96837)
### Programação de uploads
![uploads](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/dfc2d9d4-3b41-43c7-ba99-2acd6fe43590)
### Nuvem de palavras geradas a partir dos títulos dos vídeos para identificar os termos mais comuns
![cloud](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/63f8e1a4-03f7-48d5-97ea-8482ed1de5c1)


## Considerações
- Este script foi desenvolvido com base na versão 3 da API do YouTube. Qualquer atualização subsequente na API pode exigir modificações no script.
- Certifique-se de seguir as políticas de uso da API do YouTube ao utilizar este script em produção, especialmente em relação às cotas de uso da API.

## Conclusão
Este script fornece uma maneira eficiente de extrair e analisar dados do YouTube, permitindo insights valiosos sobre o desempenho de canais, vídeos individuais e interações de comentários. É útil para criadores de conteúdo, profissionais de marketing digital e pesquisadores interessados em entender melhor o ecossistema do YouTube.

# English Version

# Youtube API Analysis

This Python script is designed to extract statistical and content data from YouTube using the YouTube Data API v3. It provides insights into YouTube channels, individual videos, and comments associated with the videos.


## Reference

 - [The Vu data analytics](https://www.youtube.com/watch?v=D56_Cx36oGY)


## Authors

- [@LonguiVic](https://github.com/LonguiVic)


## Installation

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


## Documentation

[Seaborn](https://seaborn.pydata.org/installing.html)

[Matplotlib](https://matplotlib.org/stable/index.html)

[Youtube API v3](https://console.cloud.google.com/apis/library/youtube.googleapis.com?project=new-project-418921)

[Pandas](https://pandas.pydata.org/docs/)

[dateutil](https://pypi.org/project/python-dateutil/)

[nltk](https://www.nltk.org)

## How to Use the Script

### YouTube API Configuration
- You must obtain a YouTube API key. This key must be inserted into the *api_key* variable in the script.

### Specify Channel IDs
- Set the IDs of the channels you want to analyze in the *channel_ids.* list

### Script Execution
- Run the script in a Python environment. Make sure all required libraries are installed.
- It is also possible to run it through Jupyter, if you prefer.

### Results View
- The script will provide multiple views and insights into the extracted channels, videos, and comments.

## Main Script Functions

### _get_channel_stats(youtube, channel_ids)_
- This function obtains statistics from the specified channels, such as number of subscribers, total views and total videos. Returns a Pandas DataFrame with this information.

### _get_video_ids(youtube, playlist_id)_
- This function gets the video IDs of a specific playlist. Returns a list of video IDs.

### _get_video_details(youtube, video_ids)_
- This function gets specific video details such as title, description, view count, and comment count. Returns a Pandas DataFrame with this information.

### _get_comments_in_videos(youtube, video_ids)_
- This function gets the top comments from specific videos. Due to YouTube API limitations, only the first 10 comments are extracted for each video. Returns a Pandas DataFrame with the video IDs and associated comments.

## Analyzes Performed
### Best Performing Videos
![best-performing](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/dc0be1f1-a033-4dd6-8cb6-60e4c3390a6a)
### Worst Performing Videos
![worst](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/59a5146d-dd8c-4738-9b5a-de9658717fa5)
### View distribution per video
![view-dist](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/a785fe8d-7126-42c9-9c80-d0a7c58c2c9a)
### Views VS Likes and comments
![view-vs-likes](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/6af656c9-3404-43ed-8c7e-db44d4003b6e)
### Video duration
![image](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/2aaf696e-7c6e-4f9c-8f85-048b80e96837)
### Uploaded schedule
![uploads](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/dfc2d9d4-3b41-43c7-ba99-2acd6fe43590)
### Wordcloud for video titles
![cloud](https://github.com/LonguiVic/youtube-api-analysis/assets/132114257/63f8e1a4-03f7-48d5-97ea-8482ed1de5c1)


## Considerations
- This script was developed based on YouTube API version 3. Any subsequent updates to the API may require modifications to the script.
- Be sure to follow YouTube's API usage policies when using this script in production, especially regarding API usage quotas.

## Conclusion
This script provides an efficient way to extract and analyze data from YouTube, enabling valuable insights into the performance of channels, individual videos, and comment interactions. It's useful for content creators, digital marketers, and researchers interested in better understanding the YouTube ecosystem.


