# Deep Learning 2025-2026
Este repositorio contiene el material de clases (presentaciones, ejercicios y notebooks) para Deep Learning (CEIA - FIUBA)


### Requerimientos
* Lenguaje de Programación
    * Python 3.11
    * [uv](https://docs.astral.sh/uv/) para gestionar el entorno y las dependencias
* Librerías
    * Numpy
	* Pandas
	* Scikit-Learn
    * SciPy
    * PyTorch
* Consola Interactiva de Python 
    * IPython
* Herramientas
    * PyTest para tests
    * GitHub para repositorios
* IDE Recomendado 
    * PyCharm Community Edition    

### Setup del entorno

Con [uv](https://docs.astral.sh/uv/) instalado, desde la raíz del repositorio:

```bash
uv sync
```

Esto crea un `.venv` con Python 3.11 y todas las dependencias de `pyproject.toml` (incluyendo `ipykernel` y `jupyterlab` para correr los notebooks). Para registrar el kernel en Jupyter/VS Code:

```bash
uv run python -m ipykernel install --user --name=ceia-ap --display-name="Python (ceia-ap)"
```

Luego se pueden correr los notebooks con `uv run jupyter lab`, o seleccionando el kernel "Python (ceia-ap)" desde VS Code / otro editor.

> Nota: `torch` y `torchvision` están fijados por debajo de las versiones que dejaron de publicar wheels para macOS Intel (x86_64); en otras plataformas se pueden destrabar esos topes en `pyproject.toml` si hace falta.

## Contenido

### [Clase 1](clase_1/README.md) 
* Introducción a Deep Learning
* Redes Feedforward

### [Clase 2](clase_2/README.md)
* Funciones de activación
* Funciones de pérdida y de salida
* Optimización

### [Clase 3](clase_3/README.md)
* Pytorch

### [Clase 4](clase_4/README.md)
* Regularización
* Ajuste de hiperparámetros
* Embeddings

### [Clase 5](clase_5/README.md)
* Convolutional Neural Networks
    
### [Clase 6](clase_6/README.md)
* Recurrent Neural Networks
* Attention Layers

### [Clase 7](clase_7/README.md)
* Encoder-Decoder
* Autoencoder


### [Clase 8](clase_8/README.md)
* Transfer Learning
* Generative Adversarial Networks
