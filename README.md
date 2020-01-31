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