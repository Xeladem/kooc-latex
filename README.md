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

#### Add the title
#### Write down your ingredients 
#### Set the steps


### Remarks or problems?

Feel free to submit reviews or issues ;)

## Authors

Alexandre LOPES MEDA

See also the list of [contributors](https://github.com/Xeladem/kooc-latex/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the LICENSE file for details
