# Surf Status

**Surf Status** é um aplicativo focado em surfistas que deseja fornecer previsões meteorológicas e condições de ondas em tempo real. Ele integra dados de uma API de meteorologia e também utiliza o ChatGPT para interpretar essas informações de forma mais amigável e útil para surfistas, como um resumo sobre as condições do mar e das ondas.

## Objetivo

O objetivo do **Surf Status** é oferecer previsões detalhadas sobre as condições de surf, incluindo:
- **Condições climáticas**: temperatura, vento, precipitação.
- **Previsões de maré e ondas**: altura das ondas, direção e período das ondas, entre outros parâmetros marítimos.
- **Análise personalizada**: interpretação dos dados meteorológicos pelo ChatGPT para fornecer um resumo amigável e em linguagem natural sobre as condições ideais para o surf.

## Funcionalidades

- Obtenção automática da localização do usuário com base no IP.
- Integração com a API [Open Meteo](https://open-meteo.com/) para previsões climáticas e marítimas.
- Utilização do ChatGPT para gerar análises e resumos personalizados das condições de surf.
  
## Como Funciona

1. **Obtenção da Localização**: O aplicativo utiliza a função `getLocation` para identificar a latitude e longitude do usuário com base no seu IP.
  
2. **Previsão Meteorológica**: Com as coordenadas geográficas, a função `getCurrentWeather` é chamada para obter informações sobre as condições climáticas atuais, como temperatura aparente.

3. **Previsão das Ondas e Marés**: A função `getCurrentTide` coleta dados específicos sobre as condições marítimas, como altura e direção das ondas, com integração à API de marés.

4. **Interpretação pelo ChatGPT**: Utilizando a OpenAI, o bot é capaz de processar os dados brutos e gerar um resumo claro e objetivo, informando as condições ideais para o surf, tudo em português.
