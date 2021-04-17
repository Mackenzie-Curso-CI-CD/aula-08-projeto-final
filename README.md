# Aula 08 - Projeto Final

Hora de construir nosso workflow do começo ao fim!

## Requisitos

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

## Bônus

0,5 ponto extra caso:
- Identifique uma falha de segurança no código
- Implemente uma análise SAST no seu pipeline
