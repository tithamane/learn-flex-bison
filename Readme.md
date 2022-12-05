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
flex counter.l
gcc lex.yy.c -ll -o counter
./counter < counter.test
```

## pascal.l
```
flex pascal.l
gcc lex.yy.c -ll -o pascal
./pascal < pascal.test
```
