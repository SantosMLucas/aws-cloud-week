# Ola AWS Cloud Week
## Desenvolvendo back-end serverless chat
## TEMAS DE HOJE - 2023/03/01
- Backend AWS 
    Apresentados introdutóriamente diversos serviços para gerênciamento do back de uma aplicação na AWS.
- Serverless x Server Computing
    Questionamentos sobre quando usar maquinas virtuais(Ex.:EC2) ou quando utilizar serverless  (Ex.:AWS Lambda).Onde para escolha devemos levar em consideração o porte e arquitetura da aplicação para tomada de desição, bem como estudar e conhecer cada uma das soluções oferecidas.
- Desenvolver o backend do chat
    Para a aplicação proposta utilizaremos **"AWS Lambda"** e **"Amazon API Gateway"**

## AWS Lambda
   - É um serviço de computação sem servidor que permite ao desenvolvedor executar código em resposta a eventos. Como a chamada de uma API upload de arquivo, atualização de banco de dados entre outros.
   - Para um código sendo utilizados apenas a quantidade tempo de execução e quantidade de memória memória, que podem ser configurados préviamente.
    Tempo de execução variando de 3s a 15min
    
**Principais Componentes**
  - **Eventos**: Desencadeia a execução de uma função
  - **Funções**: Unidade independente da implantação
  - **Recursos**: Componentes usados pela função
  - **Caracteristicas**
    1- Aplicação deve ser construida com funções desacopladas;
    2- Statless functions: Os containers são destruidos após a execução da função, não armazenando seu estado;
    3- Cold Starts: latência para responder a um evento quando ativado sob demanda, pois em um primeiro momento ele deve efetuar dowload do seu código e iniciar a execução em novo ambiente.
## Amazon API Gateway
    É um serviço de gerenciamento de API's, possui uma extensa gama de recursos, como autorização, autenticação, limites de taxa e transformação de dados.