# SASSPractice

Extension : live Sass Compile in visual studio. Inside setting.json page (liveSassCompile) modify with 
"liveSassCompile.settings.formats": [
        {
            "format": "expanded",
            "extensionName": ".css",
            "savePath": "/dist/css"
        }
        // You can add more
        // {
        //     "format": "compressed",
        //     "extensionName": ".min.css",
        //     "savePath": "/dist/css"
        // }
        // More complex
        // {
        //     "format": "compressed",
        //     "extensionName": ".min.css",
        //     "savePath": "~/../css/"
        // }
    ]

    Variable: $ indicate a variable.
    map-get : map-get used to get value from an array. Example: 
            $font-weights: (
                "regular" : 400,
                "medium" : 500,
                "bold" : 700
            );
            font-weight: map-get($font-weights, bold );

    Nested : Example: 
            css -> .main .main__paragraph { } scss -> .main { #{&}__paragraph { } }
            css -> .main .second_paragraph { } scss -> .main { .second_paragraph { } }
            css -> .main .main__paragraph:hover { } scss -> .main { #{&}__paragraph { &:hover { } } } // #{&} used to get same prefix.