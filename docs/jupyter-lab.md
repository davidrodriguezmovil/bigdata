# 🪐 Jupyter lab

![Logo Jupyter](images/jupyter/Jupyter_logo.svg#derecha "Logo Jupyter")

Podes empregar jupyter lab dende [vscode instalando o plugin](conda-0-config-basica.md#configurar-visual-studio-code-vscode-con-conda-e-jupyterlab), sen embargo, se queres ver o caderno vía web (de xeito nativo) podes instalar jupyter e arrancalo.

## 🧾 Instalación

**Prerequisito**: [Instalar conda seguindo a guía](conda-0-config-basica.md).

1. Instala jupyterlab con conda:
``` bash
conda install jupyterlab
```

2. Arranca o jupyter lab:

    === "GNU/Linux"

        ``` bash
        mkdir -p $HOME/notebooks/
        jupyter lab --notebook-dir=$HOME/notebooks/
        ```

    === "Microsoft Windows"

        ``` bash
        mkdir %USERPROFILE%\notebooks
        jupyter lab --notebook-dir=%USERPROFILE%\notebooks
        ```

3. No caso que non se abrise automáticamente a web do navegador, vai a: <http://localhost:8888/lab>

## 🔗 Referencias

- [Web oficial de Jupyter](https://jupyter.org/)