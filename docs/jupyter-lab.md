# 🪐 Jupyter lab

![Logo Jupyter](images/jupyter/Jupyter_logo.svg#derecha "Logo Jupyter")

Podes empregar Jupyter lab dende [vscode instalando o plugin](conda-0-config-basica.md#configurar-visual-studio-code-vscode-con-conda-e-jupyterlab), sen embargo, se queres ver o caderno vía web (de xeito nativo) podes instalar Jupyter e arrancalo.

## 🧾 Instalación

- **⚠️ Prerequisito 1**: [Instalar conda seguindo a guía](conda-0-config-basica.md).
- **⚠️ Prerequisito 2**: Seleccionar o contorno onde o queiras empregar ou instalar (por exemplo **bigdata** ou **ia**): `conda activate bigdata`.

Unha vez temos conda instalado e seleccionado o contorno onde queremos instalar jupyter, facemos:

1. Instala jupyterlab con conda:
``` bash
conda install jupyterlab
```

2. Crea o cartafol `notebooks` e arranca o jupyter lab:

    === "🐧 GNU/Linux"

        ``` bash
        mkdir -p $HOME/notebooks/
        jupyter lab --notebook-dir=$HOME/notebooks/
        ```

    === "🪟 Microsoft Windows"

        **Paso 1**: Crea o directorio
        ``` bash
        mkdir %USERPROFILE%\notebooks
        ```
        **Paso 2**: Inicia Jupyter lab
        ``` bash
        jupyter lab --notebook-dir=%USERPROFILE%\notebooks
        ```

3. No caso que non se abrise automáticamente a web do navegador, vai a: <http://localhost:8888/lab>

## 📝 Volver a arrancar Jupyter

Cando xa estea instalado e queiras arrancarlo:

1. Activa o **contorno** onde estea instalado.
``` bash
conda activate bigdata
```

2. Executa Jupyter lab

    === "🐧 GNU/Linux"

        ``` bash
        jupyter lab --notebook-dir=$HOME/notebooks/
        ```

    === "🪟 Microsoft Windows"

        ``` bash
        jupyter lab --notebook-dir=%USERPROFILE%\notebooks
        ```

3. No caso que non se abrise automáticamente a web do navegador, vai a: <http://localhost:8888/lab>

## 🔗 Referencias

- [Web oficial de Jupyter](https://jupyter.org/)
- [Colab, caderno de Google na nube](https://colab.research.google.com/)