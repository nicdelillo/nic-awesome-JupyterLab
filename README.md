# nic-awesome-JupyterLab
Nic's best favourite and useful [JupyterLab](https://github.com/jupyterlab/jupyterlab) extensions and resources. 

Inspired by [awesome-jupyterlab](https://github.com/mauhai/awesome-jupyterlab). 


## Extensions
- [Monokai++ Theme](https://www.npmjs.com/package/@hokyjack/jupyterlab-monokai-plus) - A monokai dark theme similar to the Vim theme. 
- [Spellchecker](https://github.com/ijmbarr/jupyterlab_spellchecker) - Spellchecker for markdown cells.
- [Collapsable Headings](https://github.com/aquirdTurtle/Collapsible_Headings) - Collapse all the cells under the same header.
- [Table of contents generator](https://github.com/jupyterlab/jupyterlab-toc) - Nice sidebar table of content generator to navigate your notebook
- [Go to definition](https://github.com/krassowski/jupyterlab-go-to-definition) - Allows you to <kbd>Alt</kbd> + <kbd>click</kbd> on a variable or function, to jump to its definition.
- [Variable Inspector](https://github.com/lckr/jupyterlab-variableInspector) - Interactive variable inspector.
- [Execute Time](https://github.com/deshaw/jupyterlab-execute-time) - Instructions how to install [here](https://stackoverflow.com/questions/56843745/automatic-cell-execution-timing-in-jupyter-lab). Prints the cells runtime.
- [System Monitor](https://github.com/jtpio/jupyterlab-system-monitor) - Monitors cpu and memory usage see als below for Top Bar Extension
- [Top Bar Extension](https://github.com/jtpio/jupyterlab-topbar) - A topbar extension with extended tools.

#### Interactive widgets
- [jupyter-matplotlib](https://github.com/matplotlib/jupyter-matplotlib) - Make your plots interactive.
- [Voilà](https://github.com/voila-dashboards/voila) - Interactive renders for sliders, table and plots.

## Resources
- [Shortcuts for JupyterLab](https://gist.github.com/kidpixo/f4318f8c8143adee5b40#file-jupyter_shortcuts-md) - Keyboard shortcuts for JupyterNotebook.

## Other awesome lists
- [Top rated JupyterLab extensions](https://awesomeopensource.com/projects/jupyterlab-extension) - Top rated JupyterLab extensions.
- [awesome-jupyterlab](https://github.com/mauhai/awesome-jupyterlab) - A curated list of JupyterLab extensions and resources.

## More awesome links
- Progress bar using [tqdm](https://github.com/tqdm/tqdm)

## I am looking for:
Please ping me if you find one of these extensions around the globe:
- A code hider that allows to show only results and markdowns. There is one not working on the latest jupyterlab version
[jlab-hide-code ](https://github.com/AixViPMaP/jlab-hide-code).


## Tip for setting JupyterLab with conda
Install JupyterLab in your `my-env` conda environment ([doc](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html)). The idea is to run JupyterLab from your `my-env` and install python kernels from different environments, for example `my-other-env`. So that you have to install extensions only in one environment `my-env` to keep JupyterLab always up to date,

To install kernels from a different environment, install `ipykernel` ([doc](https://ipython.readthedocs.io/en/stable/install/kernel_install.html)) in each environment you want to use.
Supposing `my-env` is where your JupyterLab is, and `my-other-env` is the environment containing the kernel you want to access:

    $ conda activate my-other-env
    (my-other-env)$ conda install ipykernel
    (my-other-env)$ ipython kernel install --user --name=my-other-env --display-name="<any_name_for_kernel>" 

Where `--name` refers to the environment, while `--display-name` is the name will be displayed in the JupyterLab launcher for this kernel. If you do not pass that option, environment name will be used.
You should see a message sounding like: 

    Installed kernelspec my-other-env in User/Library/Jupyter/kernels/<any_name_for_kernel>

Now open JupyterLab from `my-env` to check if you can see the new kernel.

    (my-other-env)$ conda deactivate
    $ conda activate my-env
    (my-env)$ jupyter lab
    
NOTE: an equivalent way to install a kernel is:

    (my-other-env)$ python -m ipykernel install --user --name=my-other-env --display-name="<any_name_for_kernel>" 

#### Check your current extension list
    (my-env)$ jupyter labextension list






