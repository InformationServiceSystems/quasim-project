# Setup Instructions to Visualize the Ontology

## Protégé

### OWLViz

1. Download Protégé [here](https://protege.stanford.edu/)

1. Make sure you have a ```dot``` instance available on your machine. On macOS you can check in your terminal with the command ```whereis dot```. It will show the available ```dot``` instances on your machine. If you do not have ```dot``` installed, you can install it via ```homebrew``` or via a python package manager like ```conda``` or ```pip```.

    Either of these options is fine:

    - ```brew install graphviz```
    - ```conda install graphviz```
    - ```pip install graphviz```

    Dot will be installed alongside graphviz. 

1. After installing graphviz, run the ```whereis dot``` command again and copy the absolute path to ```dot```. 
   
   **Important**: The file is called ```dot``` and **not** ```dot.1``` or anything else.

1. Open the Protégé settings and open the tab *OWLViz*. 
   
   - Insert the path to your dot instance into *Path to DOT*
   - Increase track selection radius to 8

    ![Protégé settings](ontology_setup/protege_settings.png)

1. Lastly, if the OWLViz tab is not opened in Protégé by default, open in the menu bar *Window* -> *Tabs* -> *OWLViz*. There you can open every tab you need including OWLViz, Classes, and Object Properties.

    ![tabs](ontology_setup/owlviz_tab.png)

### Plugins

The following plugins need to be installed via the plugins manager:

- Ontology Debugger
- Pellet Reasoner Plug-in
- HermiT (should be available by default)
- OWLViz (should be available by default)

## WebVOWL

### Visualization

Another visualization possibility is [WebVOWL](http://vowl.visualdataweb.org/webvowl.html). Since it is an online tool, you do not need any setup work to do and can directly upload the ontology file in WebVOWL within the tab *Ontology*.

![webvowl](ontology_setup/webvowl_ont.png)

### Filtering

To adjust the level of detail displayed in WebVOWL, the *Filter* option is given. It provides the possibility to ignore certain parts of the ontology, like Data Properties, and to adjust the degree of collapsing. 

The whole ontology is shown when nothing is filtered and the degree of collapsing is set to 0.

![filter](ontology_setup/webvowl_filter.png)
