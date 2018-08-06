# unexpected-token. (syntax error)

When JS engine can't parse the file because I made an error in my code. It cannot even make it pass the creation

More specifically, I started something I didn't finish. Opened parenthesis I never closed, used an operator with no operand, ...

I first came accross this error studying type coercion when I tried to typeof the void operator.

I expect this error will be a real pain beacause the message isn't very helpful. It tells me there's something missing, but always
I'll have to go back through the WHOLE FILE to find where I made my mistake.

___
# Codes that thri this error

'''js
typeof void

// comments
...

'''js
typeof void;

// comments
'''

These look so similar, but are so different. Witht he semicolon JS catches the error before movong on to the ret of the file
This way it can tell me the error is on line 1, instead of having to stumble to the end and telle me something unhelpful.

__
## The fix

Well, void is an operator. It requires a value to its left, so I gave it one.
"""js
typeof void null,
'''

_null_ for  fun, but it could be anything? Doens"t matter. _void_ turns anything ti _undefined_
