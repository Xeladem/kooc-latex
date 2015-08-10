# Kooc LaTeX

Kooc is a LaTeX style to write recipe.

[![PDF Status](https://www.sharelatex.com/github/repos/Xeladem/kooc-latex/builds/latest/badge.svg)](https://www.sharelatex.com/github/repos/Xeladem/kooc-latex/builds/latest/output.pdf)
## Getting Started
### Installing

The Kooc style can be used in two way, you can put the .sty file at the root of your project and import it in your TeX file with the following command ...

```latex
\usepackage{kooc}
```

... or you can install it system wide or for the local user by putting the .sty file in the **TeXlive** folder according to your operating system. 

### Write a recipe

Now that kooc is installed, you can begin to write awesome recipes :D

#### Initiate the recipe environnement
The first step is to declare a recipe environnement, like this:

```latex
 \begin{recipe}[<recipe_type (opt)>]{<recipe_title>}{<type_and_number_of_elements>}
 
      [ ... recipe content ... ]
      
 \end{recipe}
```

for example:
```latex
 \begin{recipe}[Dessert]{My awesome recipe}{one big cake}
 
      [ ... recipe content ... ]
      
 \end{recipe}
```

The **first** optional parameter is the type of recipe (appetizer, dinner, dessert, drink, appetize,...).

The **second** one is the recipe title.

The **last** one is a decription.

#### Set the recipe parameters

First of all, you have to set the recipe parameter. There are four main parameters:
 * Total time - \settotaltime{<Time>}{<unit>}
 * Fridge time - \setfridgetime{<Time>}{<unit>}
 * Preparation time - \setpreptime{<Time>}{<unit>}
 * Leavening time - \setleavetime{<Time>}{<unit>}
 
These parameters are based on the same syntax and can be used like this:
```latex
 \settotaltime{1h}{45min}
 \setfridgetime{20}{min}
 \setpreptime{30}{min}
 \setleavetime{35}{min}
```

The is an extra command that can be used for custom parameters.
```latex
\setcustomtime{<name>}{<Time>}{<unit>}
```

Order is important !! Parameters are printed according to the declaration order.

#### Add the title

Now, you can add the title with this command:

```latex
% Make the recipe title
\makerecipetitle[<type>]{<description>}{<picture path>}{<extra info>}
```

for example:

```latex
% Make the recipe title
\makerecipetitle[over]{The is the best recipe ever !}{img/cake}{See my website <website>}
```

The optional parameter is the type of the title section. With the standard tite (no optional option), two types are available:
 * [side] - the picture is on the left side of the title.
 * [oven] - the picture is below the title.

#### Write down your ingredients

Ingredients need to be declared in a custom environnement:

```latex
 \begin{ingredients}{<ingredient list title>}{<custom bullet>}
   ...
   [ingredients here]
   ...
 \end{ingredients}
```

The first parameter is the ingredient list title. For example: "For the topping"

The second one can be left blank and is used to set the item list "bullet".

##### Add an ingredient


#### Set the steps


### Remarks or problems?

Feel free to submit reviews or issues ;)

## Authors

Alexandre LOPES MEDA

See also the list of [contributors](https://github.com/Xeladem/kooc-latex/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the LICENSE file for details
