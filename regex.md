    • /Buttercup/  -> matches any string that contains the substring Buttercup
    • /woodchucks/ is different from /Woodchucks/ 
        Note: Can solve this problem but using "[ ]" -- [ ] represent a disjunction 
    • '-' can be used to reference range 
    • /[A-Z]/ -> matches an uppercase letter
    • /[^a]/ -> returns all that do not contain an 'a'
        Note: this only true when a ^ is the first character after the open square brace
    • /?/ -> means the preceding character or nothing 
    • /[^A-Z] -> not an uppercase letter 
    • /[^Ss]/ -> not an 'S' nor 's'
    • /[^/.]/ -> not a period
    • /[e^]/ -> either 'e' or '^'
    • a^b -> the pattern 'a^b'
    • woodchucks? -> matches woodchuck's' or woodchuck
    • colou?r -> matches color or colour
    • /a*/ -> zero or any number of 'a's 
    • /[ab]*/ -> zero or more 'ab's 
    • /[0-9]+/  -> one or more sequence of digits 
    • /./ -> any character (known as a wildcard expression)
    • /beg.n/ -> any character between 'beg' & 'n'
    • /arrdvak.*arrdvak/ -> string that contains arrdvak twice
    • /^The/ -> matches the word 'The' only at the start of a line 
    • /The dog\.$/ -> matches a line that only contains 'The dog.'
    • /\bthe\b/ -> matches 'the' and not 'other' 
    • /cat|dog/ -> matches either cat or dog ('|' is a disjuntion refered to as a pipe)
    • /gupp(y|ies)/ -> matches either guppy or guppies
    • /Column_[0-9]+_*/ -> match a line with just a 'Column_[0-9]' followed by infinite number of spaces
    • /(Column_[0-9]+_*)*  -> match the whole pattern any number of times
    • /\b[tT]he\b/ -> will return The or the due to word boundry
    • /[^a-zA-Z][tT]he[^a-zA-Z]/ -> doesn't begin or end with any alphabetic characters
    • /(^|^a-zA-Z)[tT]he(^a-zA-Z|$)/ -> accepts the/The alone
    • \d -> shorthand for [0-9]
    • \D -> shorthand for [^0-9]
    • \w -> any alphanumeric/_
    • \W -> shorthand for [^\w] = "!!!"
    • \s -> whitespace\tab
    • \S -> Non-(whitespace/tab)\
    • \* -> Kleene star
    • + -> 1 or more occurences
    • ? -> may or may not occur
    • {n} -> exactly n appearances of a character
    • {n, m} -> btwn n and m occurences of a character
    • {n, } -> at least n occurences of a character
    • s/colour/color/ -> s/regexp/pattern/
    • s/([0-9]+)/<\1>/ -> 9 => <9>
    • /the (.*)er they were, the \1er they will be/ -> the bigger they were the bigger they will be
    • \1 -> refered to as registers