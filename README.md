# TruthTable-Generator
A LaTex truth tables generator implemented using python

A tree is used to represent the structure of a logical proposition. The buit methods take strings as input. The following operators are supported:

- Negation `¬` 
- Conjunction `^`
- Disjunction `|`
- Conditional `->`
- Biconditional `<->`

Parentheses must be used to avoid ambiguity. For example, `a^b->c` must be written as `"(a^b)->c"`. Also, all variables must be letters of the alphabet.

The available functions to create truth tables are `texTT` and `mainTexTT`. 

`texTT` is used to create a single truth table and takes the following arguments:
```
    texTT(filename, str_expr, standalone)
```
where `filename` is the name of the file to create, `str_expr` is a string with the logical expression to calculate and `standalone` is a variable of type `bool` that specifies whether or not to include packages and the `document` environment in the file.

`mainTexTT` is used to add several TruthTables to the same LaTex main document and takes the following arguments:
```
    texTT(filename, exprs)
```
where `filename` is the name of the file to create and `exprs` is a list that contains several strings with the logical expressions to calculate.

---

Se utliza un árbol para representar la la estructura de una proposición lógica. Los métodos incluidos toman cadenas de caracteres como entrada. Están considerados los siguientes operadores:

- Negación `¬` 
- Conjunción `^`
- Disyunción `|`
- Condicional `->`
- Bicondicional `<->`

Se deben usar paréntesis para evitar ambigüedades. Por ejemplo, `a^b` debe escribirse como `"(a^b)->c"`. También, las variables deben ser letras del alfabeto.

Las funciones disponibles para generar tablas de verdad, son`texTT` y `mainTexTT`. 

`texTT` toma los siguientes argumentos:
```
    texTT(filename, str_expr, standalone)
```
donde `filename` es el nombre del archivo a crear, `str_expr` es una cadena que contiene la proposición a calcular y `standalone` es una variable de tipo `bool` que especifica si se van a incluir o no los paquetes y el ambiente `document` en el archivo.

`mainTexTT` se usa para agregar varias tablas de verdad en el mismo documento base de LaTex y toma los siguientes argumentos:
```
    texTT(filename, exprs)
```
donde `filename` es el nombre del archivo a crear y `exprs` es una lista que contiene varias cadenas de caracteres con las proposiciones a calcular.
