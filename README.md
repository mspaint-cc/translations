# Translations
This is the translation mappings for mspaint. [Languages.json](https://github.com/mspaint-cc/translations/blob/main/Languages.json) contains the mappings of all the languages available.

# Contributing
Keep in mind that each file is named based on the [IETF BCP 47 language tag standard](https://en.wikipedia.org/wiki/IETF_language_tag). Please follow the conventions found in the translation files!

You can use one of the files in `/translations/` as a template. You can create a PR to submit changes and add new language support. Please do not spam the PRs with spam.

# Testing
To test out your language in game, you can put the `.json` file in your executor's workspace folder and run this **BEFORE** loading mspaint:

```lua
getgenv().environement = "translator_env"
getgenv().overrideLanguage = "en"
getgenv().language = {
    ["en"] = {
        NativeName = "English",
        EnglishName = "English",
        Path = "file_in_executor_workspace.json"
    }
}
```
> Missing translations are printed in the Developer console (F9, /console)
## Language Info
> [!IMPORTANT]
> NativeName is the name of the language in the native language, example for french:
> ```lua
> getgenv().language = {
>     ["fr"] = {
>         NativeName = "Français",
>         EnglishName = "French",
>         Path = "fr.json"
>     }
> }
> ```


