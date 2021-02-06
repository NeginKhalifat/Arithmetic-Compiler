# Arithmetic-Compiler
simple compiler to convert the arithmetic expressions to a readable format to human.
supports for maximum `6 digits integer`.


### To Run ###  
after installing flex and bison following bellow commands:

``` 
$ flex .\lexical.l
$ bison -d .\parser.y
$ gcc .\lex.yy.c .\parser.tab.c -o calc
$ .\calc.exe
```

### sample input/output
* input:<br/>
```
12+763*876521
```

* expected output:  
```
Assign SevHun_SixTen_Thr Mul (EigHun_SevTen_Six)Tou_FivHun_TwoTen_One to t1
Assign OneTen_Two Plu t1 to t2
Print t2
```
