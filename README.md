# Modelo Preditivo para Aprovação de Crédito

Os modelos de score de créditos são utilizados para calcular a probabilidade de inadimplência. Essa ferramenta possibilita que as empresas aprovem ou não o empréstimo com base no risco oferecido por um cliente.

## Sobre os Dados:

| Variável                              | Tipo    | Descrição                                                    |
| ------------------------------------- | ------- | ------------------------------------------------------------ |
| idade                                 | integer | A idade do cliente                                           |
| numero_de_dependentes                 | integer | O número de pessoas dependentes do cliente                   |
| salario_mensal                        | float   | Salário mensal do cliente                                    |
| numero_emprestimos_imobiliarios       | integer | Quantidade de empréstimos imobiliários que o cliente possui em aberto |
| numero_vezes_passou_90_dias           | integer | Número de vezes que o tomador passou mais de 90 dias em atraso |
| util_linhas_inseguras                 | float   | Quanto que o cliente está usando, relativamente ao limite dele, de linhas de crédito que não são seguradas por qualquer bem do tomador<br/>e.g: imóveis, carros, etc. |
| vezes_passou_de_30_59_dias            | integer | Número de vezes que o cliente atrasou, entre 30 e 59 dias, o pagamento de um empréstimo |
| razao_debito                          | float   | Razão entre as dívidas e o patrimônio do tomador. razão débito = Dividas/Patrimônio |
| numero_linhas_crdto_aberto            | integer | Número de empréstimos em aberto pelo cliente                 |
| numero_de_vezes_que_passou_60_89_dias | integer | Número de vezes que o cliente atrasou, entre 60 e 89 dias, o pagamento de um empréstimo |
| inadimplente                          | bool    | A classe ao qual o cliente pertence. <br>e.g: True (inadimplente) |

## Objetivo

O objetivo desse estudo é construir um modelo preditivo utilizando o dataset `treino.csv` . As previsões realizadas no `treinamento.csv` serão armazenadas em uma nova coluna, chamada __inadimplente__.