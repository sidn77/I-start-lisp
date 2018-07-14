# I-start-lisp
My journey with Lisp (Common Lisp)

## Tools used:
- Emacs
- Slime

## My Notes

- Macros, what are they ? how are they evaluated ?

  >Macros in lisp are not anything like the ones in C/C++. 
  They are a neat way of getting the interpreter to generate code for you.
  Syntax : (defmacro [name] ([parameters]) ([body]))
  When the Lisp interpreter identifies a macro it does not evaluate its parameters, it just passes over them.
  Then when the code in the body is evaluated at that time the parameters can be modified, and then when the 
  modified parameters are returned by the macro they are evaluated by the interpreter.
