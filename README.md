A tree is used to represent the structure of a logical proposition. The buit methods take strings as input. The following operators are supported:

- Negation `¬` 
- Conjunction `^`
- Disjunction `|`
- Conditional `->`
- Biconditional `<->`

Parentheses must be used to avoid ambiguity. For example, `a^b->c` must be written as `"(a^b)->c"`. Also, all variables must be letters of the alphabet.

The method that is used to create the truth tables is `texTT`.

`texTT` takes the following arguments:
```
    texTT(filename, str_expr, standalone)
```
Where:
- `filename` is the name of the file to create.
- `str_expr` is either a string with the logical expression to calculate or a list of such strings (if there are multiple tables to generate).
- `standalone` is a variable of type `bool` that specifies whether or not to include packages and the `document` environment in the file.
It creates de file in `./output`.

---

Se utliza un árbol para representar la la estructura de una proposición lógica. Los métodos incluidos toman cadenas de caracteres como entrada. Están considerados los siguientes operadores:

- Negación `¬` 
- Conjunción `^`
- Disyunción `|`
- Condicional `->`
- Bicondicional `<->`

Se deben usar paréntesis para evitar ambigüedades. Por ejemplo, `a^b->c` debe escribirse como `"(a^b)->c"`. También, las variables deben ser letras del alfabeto.

El método utilizado para crear las tablas es `texTT`.

`texTT` toma los siguientes argumentos:
```
    texTT(filename, str_expr, standalone)
```
Where:
- `filename` es el nombre del archivo que se va a crear.
- `str_expr` es ya sea una cadena con una expresión lógica, o una lista con cadenas de esa forma.
- `standalone` es una variable de tipo `bool` que especifica si hay que incluir los paquetes y el ambiente `document` en el archivo.
It creates de file in `./output`.
