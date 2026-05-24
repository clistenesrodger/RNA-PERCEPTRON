# Classificação Breast Cancer (Perceptron do zero)

Este projeto usa o dataset **Breast Cancer Wisconsin (Diagnostic)** via `scikit-learn` e executa um perceptron implementado “na mão” no notebook. O fluxo inclui normalização (z-score), validação cruzada k-fold e exportação de resultados.

## Requisitos

- Linux
- Python 3

## 1) Criar e ativar ambiente virtual

Na pasta do projeto:

```bash
python3 -m venv venv
source venv/bin/activate
```

Atualize o `pip` (recomendado):

```bash
python -m pip install --upgrade pip
```

## 2) Instalar dependências

Com a `venv` ativada:

```bash
pip install -r requirements.txt
```

> Observação: `matplotlib` pode ser usado para gráficos, mas o notebook atual foca nas tabelas e métricas do perceptron.

## 3) Usar o kernel do Jupyter no VS Code

### Opção A — Abrindo o notebook e escolhendo o kernel

1. Abra o arquivo `jupyter.ipynb` no VS Code.
2. No canto superior direito do notebook, clique em **Select Kernel** (Selecionar Kernel).
3. Selecione o Python da sua `venv` (normalmente algo como `venv (Python 3.x)` ou o caminho `./venv/bin/python`).
4. Execute as células na ordem.

### Opção B — Se o kernel da `venv` não aparecer

Instale o kernel do IPython dentro da `venv`:

```bash
source venv/bin/activate
pip install ipykernel
python -m ipykernel install --user --name breastcancer-venv --display-name "breastcancer-venv"
```

Depois volte ao `jupyter.ipynb` e selecione o kernel **breastcancer-venv**.

## 4) Arquivos gerados

Ao executar o notebook, serão gerados:

- `predicoes_resultados.csv` (tabela com real vs predito e coluna de acerto)

Esses arquivos estão ignorados no Git pelo `.gitignore`.
