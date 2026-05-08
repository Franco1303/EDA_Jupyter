# EDA CSS Magdalena - Python 3.9

Notebook ajustado para Python 3.9.x, Jupyter Book 0.15.1 y HTML local.

## Crear ambiente

```powershell
conda create -n frank_eda python=3.9 -y
conda activate frank_eda
pip install -r requirements_eda.txt
python -m ipykernel install --user --name frank_eda --display-name "Python 3.9 - Frank EDA"
```

## Construir HTML local

Copia los archivos de datos necesarios en esta misma carpeta y ejecuta:

```powershell
jupyter-book clean .
jupyter-book build .
start _build\html\index.html
```

El `_config.yml` usa `execute_notebooks: force` para regenerar las salidas y embeber las gráficas Plotly.
