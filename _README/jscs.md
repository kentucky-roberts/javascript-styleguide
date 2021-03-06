# JSCS

Use an Options File

Use JSCS for checking your coding styles your JavaScript and be sure to customize the JSCS options file and include in source control. See the JSCS docs for details on the options.

Why?: Provides a first alert prior to committing any code to source control.

Why?: Provides consistency across your team.

````{
{
    "excludeFiles": ["node_modules/**", "bower_components/**"],

    "requireCurlyBraces": [
        "if",
        "else",
        "for",
        "while",
        "do",
        "try",
        "catch"
    ],
    "requireOperatorBeforeLineBreak": true,
    "requireCamelCaseOrUpperCaseIdentifiers": true,
    "maximumLineLength": {
      "value": 100,
      "allowComments": true,
      "allowRegex": true
    },
    "validateIndentation": 4,
    "validateQuoteMarks": "'",

    "disallowMultipleLineStrings": true,
    "disallowMixedSpacesAndTabs": true,
    "disallowTrailingWhitespace": true,
    "disallowSpaceAfterPrefixUnaryOperators": true,
    "disallowMultipleVarDecl": null,

    "requireSpaceAfterKeywords": [
      "if",
      "else",
      "for",
      "while",
      "do",
      "switch",
      "return",
      "try",
      "catch"
    ],
    "requireSpaceBeforeBinaryOperators": [
        "=", "+=", "-=", "*=", "/=", "%=", "<<=", ">>=", ">>>=",
        "&=", "|=", "^=", "+=",

        "+", "-", "*", "/", "%", "<<", ">>", ">>>", "&",
        "|", "^", "&&", "||", "===", "==", ">=",
        "<=", "<", ">", "!=", "!=="
    ],
    "requireSpaceAfterBinaryOperators": true,
    "requireSpacesInConditionalExpression": true,
    "requireSpaceBeforeBlockStatements": true,
    "requireLineFeedAtFileEnd": true,
    "disallowSpacesInsideObjectBrackets": "all",
    "disallowSpacesInsideArrayBrackets": "all",
    "disallowSpacesInsideParentheses": true,

    "jsDoc": {
        "checkAnnotations": true,
        "checkParamNames": true,
        "requireParamTypes": true,
        "checkReturnTypes": true,
        "checkTypes": true
    },

    "disallowMultipleLineBreaks": true,

    "disallowCommaBeforeLineBreak": null,
    "disallowDanglingUnderscores": null,
    "disallowEmptyBlocks": null,
    "disallowTrailingComma": null,
    "requireCommaBeforeLineBreak": null,
    "requireDotNotation": null,
    "requireMultipleVarDecl": null,
    "requireParenthesesAroundIIFE": true
}
}````