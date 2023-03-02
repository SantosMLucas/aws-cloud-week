# Ola AWS Cloud Week
## Desenvolvendo back-end serverless chat
## TEMAS DE HOJE - 2023/03/01
- Backend AWS 
    Apresentados introdut�riamente diversos servi�os para ger�nciamento do back de uma aplica��o na AWS.
- Serverless x Server Computing
    Questionamentos sobre quando usar maquinas virtuais(Ex.:EC2) ou quando utilizar serverless  (Ex.:AWS Lambda).Onde para escolha devemos levar em considera��o o porte e arquitetura da aplica��o para tomada de desi��o, bem como estudar e conhecer cada uma das solu��es oferecidas.
- Desenvolver o backend do chat
    Para a aplica��o proposta utilizaremos **"AWS Lambda"** e **"Amazon API Gateway"**

## AWS Lambda
   - � um servi�o de computa��o sem servidor que permite ao desenvolvedor executar c�digo em resposta a eventos. Como a chamada de uma API upload de arquivo, atualiza��o de banco de dados entre outros.
   - Para um c�digo sendo utilizados apenas a quantidade tempo de execu��o e quantidade de mem�ria mem�ria, que podem ser configurados pr�viamente.
    Tempo de execu��o variando de 3s a 15min
    
**Principais Componentes**
  - **Eventos**: Desencadeia a execu��o de uma fun��o
  - **Fun��es**: Unidade independente da implanta��o
  - **Recursos**: Componentes usados pela fun��o
  - **Caracteristicas**
    1- Aplica��o deve ser construida com fun��es desacopladas;
    2- Statless functions: Os containers s�o destruidos ap�s a execu��o da fun��o, n�o armazenando seu estado;
    3- Cold Starts: lat�ncia para responder a um evento quando ativado sob demanda, pois em um primeiro momento ele deve efetuar dowload do seu c�digo e iniciar a execu��o em novo ambiente.
## Amazon API Gateway
    � um servi�o de gerenciamento de API's, possui uma extensa gama de recursos, como autoriza��o, autentica��o, limites de taxa e transforma��o de dados.