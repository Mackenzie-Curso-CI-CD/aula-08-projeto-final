# Aula 08 - Projeto Final

Hora de construir nosso workflow do começo ao fim!

![scary-gif](https://media.giphy.com/media/12RfP2odT4hEOI/source.gif)
   
## Requisitos obrigatórios

1. Jobs obrigatórios
   1. Build e test
   2. Linter (ver exemplo)
   3. Deploy homologacao
   4. Deploy producao
2. Uso de **variáveis de ambiente** quando for necessário armazenar nome da aplicação, versão do framework, etc
3. Uso de **secrets** para tokens de API, senha de BD, credenciais de autenticação
4. Uso de **ambientes** (`environments`) para separar secrets dos ambientes de Homologação e Produção
5. Ao menos 1 aprovação para deploy em produção
6. Branch `main` protegido. Status obrigatórios
   1. Build e test
   2. Deploy homologação
7. Ao menos 1 revisão de código obrigatória no Pull Request

### ❗ Importante

O deploy pode ser feito em qualquer cloud de sua preferência. Recomendados: **Azure e Heroku**

## Dados importantes

**Strings de conexão do Banco de Dados**
- **Homologação:**

```javascript
"mongodb+srv://dba:s2OuCobCglTtech6@cluster0.uiv1l.mongodb.net/local_library_dev?retryWrites=true"
```

- **Produção:** 

```javascript
"mongodb+srv://dba:s2OuCobCglTtech6@cluster0.uiv1l.mongodb.net/local_library?retryWrites=true"
```


**Comandos de execução da aplicação**

- **Dev**

```bash
MONGODB_URI=<string_de_conexao_do_banco> npm run devstart
```

- **Prod**

```bash
MONGODB_URI=<string_de_conexao_do_banco> npm run start
```

## Bônus

0,5 ponto extra para cada item abaixo:
- Identifique ao menos uma falha de segurança no código/aplicação
- Implemente uma análise SAST no seu pipeline

![good-luck](https://media.giphy.com/media/QXPfCbIa2VLI5lbzEP/giphy.gif)
