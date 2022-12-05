# Running

### Note - lex file structure
```
definitions
%%
rules
%%
user code
```

### GCC Flags
- `-ll` -> (link lex library for "yylex") https://stackoverflow.com/questions/15732155/what-is-ll-gccs-flag

## counter.l
```
flex -o counter.yy.c counter.l
gcc counter.yy.c -ll -o counter.run
./counter.run < counter.code
```

## pascal.l
```
flex -o pascal.yy.c pascal.l
gcc pascal.yy.c -ll -o pascal.run
./pascal.run < pascal.code
```
