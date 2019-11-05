# nic-awesome-JupyterLab
Nic's best favourite and useful JupyterLab extensions and resources. 

Inspired by [awesome-jupyterlab](https://github.com/mauhai/awesome-jupyterlab). 


## Extensions
- [Spellchecker](https://github.com/ijmbarr/jupyterlab_spellchecker) - Spellchecker for markdown cells.
- [Collapsable Headings](https://github.com/aquirdTurtle/Collapsible_Headings) - Collapse all the cells under the same header.
- [Table of contents generator](https://github.com/jupyterlab/jupyterlab-toc) - Nice sidebar table of content generator to navigate your notebook
- [Go to definition](https://github.com/krassowski/jupyterlab-go-to-definition) - Allows you to <kbd>Alt</kbd> + <kbd>click</kbd> on a variable or function, to jump to its definition.
- [Variable Inspector](https://github.com/lckr/jupyterlab-variableInspector) - Interactive variable inspector.

#### Interactive widgets
- [jupyter-matplotlib](https://github.com/matplotlib/jupyter-matplotlib) - Make your plots interactive.
- [Voilà](https://github.com/voila-dashboards/voila) - Interactive renders for sliders, table and plots.

## Resources
- [Shortcuts for JupyterLab](https://gist.github.com/kidpixo/f4318f8c8143adee5b40#file-jupyter_shortcuts-md). 
Keyboard shortcuts for JupyterNotebook.

## Other awesome lists
- [Top rated JupyterLab extensions](https://awesomeopensource.com/projects/jupyterlab-extension) -T op rated JupyterLab extensions.
- [awesome-jupyterlab](https://github.com/mauhai/awesome-jupyterlab) - A curated list of JupyterLab extensions and resources.



## I am looking for:
- Progress bar or cells runtime printer. Similar to what you can do using [tqdm](https://github.com/tqdm/tqdm), but automatic.
- An code hider that allows to show only results and markdowns. There one not working on new jupyterlab version
[jlab-hide-code ](https://github.com/AixViPMaP/jlab-hide-code).


## Tip for setting JupyterLab with conda
[Install](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html) JupyterLab in your `myenv` conda environment. To keep JupyterLab always up to date, the idea is to run JupyterLab from your `myenv` and install kernels from different environments, for example `my-other-env`.

To install kernels from a different environment, install `iperkernel` ([iperkernel doc](https://ipython.readthedocs.io/en/stable/install/kernel_install.html) in each environment you want to use.
To access kernels from environment to a differnt one
Supposing `myenv` is where your JupyterLab is, and `my-other-env` is the environment containing the kernel you want to access:

    $ conda activate my-other-enve
    (my-other-env)$ ipython kernel install --user --name=my-other-env

You should see a message sounding like: 

    Installed kernelspec my-other-enve in User/Library/Jupyter/kernels/my-other-env

Now open JupyterLab from `myenv` to check if you can see the new kernel.

    (my-other-env)$ conda deactivate
    $ conda activate myenv
    (my-env)$ jupyter lab

#### Check your current extension list
    (my-env)$ jupyter labextension list






