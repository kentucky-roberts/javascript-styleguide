# JS Hint

Use an Options File

[Style Y230]

Use JS Hint for linting your JavaScript and be sure to customize the JS Hint options file and include in source control. See the JS Hint docs for details on the options.

Why?: Provides a first alert prior to committing any code to source control.

Why?: Provides consistency across your team.


````{
{
    "bitwise": true,
    "camelcase": true,
    "curly": true,
    "eqeqeq": true,
    "es3": false,
    "forin": true,
    "freeze": true,
    "immed": true,
    "indent": 4,
    "latedef": "nofunc",
    "newcap": true,
    "noarg": true,
    "noempty": true,
    "nonbsp": true,
    "nonew": true,
    "plusplus": false,
    "quotmark": "single",
    "undef": true,
    "unused": false,
    "strict": false,
    "maxparams": 10,
    "maxdepth": 5,
    "maxstatements": 40,
    "maxcomplexity": 8,
    "maxlen": 120,

    "asi": false,
    "boss": false,
    "debug": false,
    "eqnull": true,
    "esnext": false,
    "evil": false,
    "expr": false,
    "funcscope": false,
    "globalstrict": false,
    "iterator": false,
    "lastsemic": false,
    "laxbreak": false,
    "laxcomma": false,
    "loopfunc": true,
    "maxerr": false,
    "moz": false,
    "multistr": false,
    "notypeof": false,
    "proto": false,
    "scripturl": false,
    "shadow": false,
    "sub": true,
    "supernew": false,
    "validthis": false,
    "noyield": false,

    "browser": true,
    "node": true,

    "globals": {
        "angular": false,
        "$": false
    }
}
}````