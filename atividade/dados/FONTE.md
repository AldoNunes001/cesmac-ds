# Procedência dos dados

- **Base:** Dry Bean, UCI Machine Learning Repository, identificador 602.
- **Página:** https://archive.ics.uci.edu/dataset/602/dry+bean+dataset
- **DOI da base:** https://doi.org/10.24432/C50S4B
- **Autores do estudo:** Murat Koklu e Ilker Ali Ozkan.
- **Referência:** Koklu, M.; Ozkan, I. A. (2020). *Multiclass classification of
  dry beans using computer vision and machine learning techniques*. Computers
  and Electronics in Agriculture, 174, 105507.
  https://doi.org/10.1016/j.compag.2020.105507
- **Licença informada pela UCI:** Creative Commons Attribution 4.0 International
  ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
- **Data de obtenção:** 05/11/2026.
- **Download oficial:** https://archive.ics.uci.edu/static/public/602/dry%2Bbean%2Bdataset.zip

## Preparação da cópia distribuída

O arquivo `DryBeanDataset/Dry_Bean_Dataset.arff` do ZIP oficial foi convertido
para `dry_bean.csv`, com codificação UTF-8, vírgula como separador e ponto decimal.
Foram mantidos os 13.611 registros, a ordem das linhas, os 16 atributos e a coluna
`Class`. Os valores textuais das células foram preservados na conversão.
Não foram removidas duplicatas, corrigidos valores, reamostradas classes ou
adicionadas colunas. O dicionário em português é material de apoio desta atividade.

Os nomes `AspectRation` e `roundness` foram mantidos exatamente como aparecem
no ARFF, mesmo que a página da UCI use outra grafia em partes da documentação.
Os fatores `ShapeFactor1` a `ShapeFactor4` foram descritos sem inventar fórmulas
que não constam na descrição resumida da UCI.

O alvo binário deve ser construído pelos alunos: `1` para `Class == "HOROZ"`
e `0` para as demais variedades. A coluna `Class` original permanece no CSV
para uso futuro com classificação multiclasse.

## Integridade

SHA-256 do ZIP oficial obtido:

```text
0a64eff5be87f48c3dbbfc0a12a56c5d5b5167ef8e61cd45d69b3e7c7130c06f
```

SHA-256 do CSV distribuído:

```text
41457e55bb07426ecf613c95b9429660e2c4c43ecf4673d8b5c7a69ac88055ef
```
