# Atividade extra — Regressão logística

**Valor: até 1,0 ponto extra.** Individual ou em equipes de até **5 integrantes**.
O prazo será informado pelo professor.

Abra `Atividade_Extra_Regressao_Logistica.ipynb`. O notebook contém o enunciado,
os blocos para os alunos completarem, perguntas de interpretação, a rubrica e
o checklist de entrega. As etapas são diagnóstico, alvo binário, separação dos
dados, EDA, referência majoritária, regressão logística e avaliação.

## Arquivos

- `Atividade_Extra_Regressao_Logistica.ipynb`: versão do aluno, sem respostas.
- `dados/dry_bean.csv`: base real completa, com os rótulos originais.
- `dados/dicionario_dry_bean.csv`: descrição das 17 colunas em português.
- `dados/FONTE.md`: procedência, licença e conversão do arquivo original.
- `requirements.txt`: bibliotecas para execução local.

## Execução

**Jupyter:** abra o notebook dentro de `atividade/` ou a partir da raiz do
projeto. Para instalar as dependências, execute no terminal, dentro de `atividade/`:

```bash
python -m pip install -r requirements.txt
python -m jupyterlab
```

Use Python 3.10 ou superior. Os CSVs locais permitem trabalhar sem internet
depois da instalação das bibliotecas.

**Google Colab:** abra o `.ipynb` e envie `dry_bean.csv` e
`dicionario_dry_bean.csv` para a área de arquivos da sessão. O carregador encontra
os dois CSVs na pasta atual. Os arquivos precisam ser enviados novamente se a
sessão do Colab for reiniciada.

Os campos `TODO` devem ser preenchidos pelos estudantes. As verificações desses
campos só passam depois que as respectivas tarefas forem implementadas.

## Escolha da base e escopo

A [Dry Bean, da UCI](https://archive.ics.uci.edu/dataset/602/dry+bean+dataset)
tem 13.611 registros, 16 medidas numéricas e sete variedades de feijão.
Nesta atividade, a classe positiva é **HOROZ** e a negativa reúne as outras seis
variedades. A classe positiva representa aproximadamente 14% da base original,
sem reamostragem artificial.

O CSV mantém `Class` para permitir uma atividade multiclasse no futuro. Nesta
entrega, `Class` é usada apenas para construir `y`; não pode entrar nas variáveis
preditoras. O alvo e os dados fornecidos não foram balanceados nem deduplicados.

O protocolo exige a retirada de duplicatas exatas antes da separação, EDA
detalhada somente no treino, padronização em `Pipeline` e escolha entre duas
regressões logísticas pela média de F1 em validação cruzada estratificada.
O teste fica reservado para avaliar a opção escolhida e a referência majoritária.
A nota depende do procedimento e da interpretação, sem exigir uma pontuação
mínima de desempenho do modelo.

## Rubrica

| Etapa | Pontos |
|---|---:|
| 1. Contexto, diagnóstico e alvo | 0,10 |
| 2. Separação dos dados | 0,10 |
| 3. Análise exploratória | 0,25 |
| 4. Referência majoritária | 0,10 |
| 5. Regressão logística e validação | 0,20 |
| 6. Avaliação final | 0,15 |
| 7. Conclusão e organização da entrega | 0,10 |
| **Total** | **1,00** |

Consulte os critérios detalhados no notebook. Os desafios opcionais não aumentam
o limite de 1,0 ponto extra.
