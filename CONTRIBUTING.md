# Regras de uso da organização HymenopteraLab-MZUSP

Tudo o que o laboratório produz — protocolos, scripts, pipelines, análises de teses e dissertações, materiais de ensino — fica nesta organização. Assim o trabalho continua acessível depois que cada pessoa sai, e conseguimos reportar o que foi produzido a cada financiador.

## 1. Criar um repositório

1. Na página do [template-hymenopteralab](https://github.com/HymenopteraLab-MZUSP/template-hymenopteralab), clique em **Use this template → Create a new repository**.
2. **Owner:** `HymenopteraLab-MZUSP` (nunca a conta pessoal).
3. **Nome:** prefixo + tema, em minúsculas, com hífens:

| Prefixo | Uso | Exemplo |
| --- | --- | --- |
| `pop-` / `protocolo-` | protocolos de bancada, coleção ou campo | `protocolo-extracao-dna-museu` |
| `pipeline-` | fluxos de análise reutilizáveis | `pipeline-uce-hymenoptera` |
| `analise-` | análises de tese, dissertação ou artigo | `analise-ectatomma-revisao` |
| `dados-` | dados pequenos e metadados | `dados-coletas-araca` |
| `ensino-` | cursos e materiais didáticos | `ensino-taxonomia-formicidae` |

4. **Visibilidade:** comece como *Private*. Torne público ao publicar o trabalho, ou antes, com acordo da orientação.
5. Preencha o `README.md` e o `CITATION.cff`, inclusive a seção **Financiamento**.

## 2. Topics obrigatórios

Na página do repositório, clique na engrenagem ao lado de **About** e adicione:

- **Tipo:** `protocolo`, `pipeline`, `analise`, `dados` ou `ensino`
- **Responsável:** `nome-sobrenome` (ex.: `diego-matielo`)
- **Financiamento**, um topic por processo: agência + número, sem barras (ex.: `fapesp-2023-12809-0`, `capes`, `cnpq-123456-2024-0`)
- **Tema** (opcional): `formicidae`, `uce`, `biogeografia`…

Topics só aceitam letras minúsculas, números e hífens.

## 3. Financiamento

Na seção **Financiamento** do README, cite o projeto do laboratório **e** a sua bolsa, com nome completo da agência e número do processo, exatamente como exigido nas publicações. A FAPESP exige também a frase: *"As opiniões, hipóteses e conclusões ou recomendações expressas neste material são de responsabilidade dos autores e não necessariamente refletem a visão da FAPESP."*

## 4. Dados

- Não versionar arquivos acima de 50 MB (o GitHub recusa acima de 100 MB). Dados brutos vão para SRA, GenBank, Zenodo ou Dryad, com o link no README.
- Nunca versionar senhas, tokens, dados pessoais ou coordenadas precisas de espécies ameaçadas.
- Material com acesso ao patrimônio genético precisa de cadastro no SisGen antes de publicação (ver POP-HYM-15).

## 5. Versões e DOI

Ao submeter um artigo ou depositar uma tese, crie um *release* (**Releases → Draft a new release**, ex.: `v1.0.0`). A integração com o Zenodo gera um DOI. Atualize o README, o `CITATION.cff` e a tabela de produtos do perfil da organização.

## 6. Ao sair do laboratório

- O repositório permanece na organização; o acesso de escrita é encerrado e a autoria continua registrada no histórico e no `CITATION.cff`.
- Antes do desligamento: README completo, último *release* criado e dados brutos depositados.
- Repositórios antigos em contas pessoais podem ser transferidos em **Settings → Transfer ownership**.
