> [!tldr]- - [ ] Correct the code block shading starting at 1.1 for better readability.
> C:\Users\ehrrsn7\Code\object-oriented-programming\cpp\Unit-1\Chapter-1.1\1.1-Defensive-Programming.ai.md
> ```
>   195,1: <!-- TODO: shade these code blocks (multiple in this file) -->
> ```

> [!tldr]- - [ ] Continue aligning headers for consistency starting at 1.3. Look for and format any unformatted code blocks.
> C:\Users\ehrrsn7\Code\object-oriented-programming\cpp\Unit-1\Chapter-1.3\1.3-Structures.ai.md
> ```
>   49,1: <!-- TODO: continue aligning headers -->
>   384,1: <!-- TODO: Continue looking for unformatted code -->
> ```

> [!tldr]- - [ ] Import Unit 2 assets and update the classname in the markdown. Continue for Units 3-4 as well.
> C:\Users\ehrrsn7\Code\object-oriented-programming\cpp\Unit-2\Chapter-2.0\2.0-Encapsulation-Design.ai.md
> ```
>   26,46: # Unit 2. Encapsulation {.unit-1-background} <!-- todo: import unit 2 assets and update classname -->
> ```

> [!tldr]- - [x] Bulk replace all occurrences of & with the correct symbol (likely &amp; or similar).
> C:\Users\ehrrsn7\Code\object-oriented-programming\cpp\Unit-2\Chapter-2.3\2.3-Accessors-&-Mutators.ai.md
> ```
>   15,28: # 2.3 Accessors & Mutators <!-- TODO: bulk replace & with & -->
> ```

> [!tldr]- - [ ] Repeat the conversion process used here for the CS 124 course, as the workflow is now established.
> C:\Users\ehrrsn7\Code\object-oriented-programming\cpp\Unit-4\Chapter-4.6\4.6-Standard-Template-Library.ai.md
> ```
>   444,1: <!-- TODO: repeat this conversion process for CS 124 too (should go a lot quicker now that we've got the workflow down)-->
> ```

> [!tldr]-- [x] Can't convert to PDF's (it poops out like 2 files in)
> here is a TypeError related to a null value in the markdown-extended extension. This may be due to an invalid or missing image/file path in your markdown files.
> When running {
>   "key": "",
>   "command": "markdownExtended.exportWorkspace"
> }
> We get the following error:
> ```
> Cannot read properties of null (reading 'replace')
> TypeError: Cannot read properties of null (reading 'replace')
>     at normalize (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\node_modules\mimoza\index.js:32:21)
>     at Mimoza.getMimeType (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\node_modules\mimoza\index.js:158:21)
>     at Mimoza._getMimeType [as getMimeType] (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\node_modules\mimoza\index.js:206:18)
>     at html5_embed_renderer (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\node_modules\markdown-it-html5-embed\lib\index.js:41:25)
>     at md.renderer.rules.image (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\node_modules\markdown-it-html5-embed\lib\index.js:108:14)
>     at Object.e.renderer.rules.image (c:\Users\ehrrsn7\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\markdown-language-features\dist\extension.js:2:1071636)
>     at s.renderInline (c:\Users\ehrrsn7\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\markdown-language-features\dist\extension.js:2:197186)
>     at s.render (c:\Users\ehrrsn7\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\markdown-language-features\dist\extension.js:2:197590)
>     at s.e.renderer.render [as render] (c:\Users\ehrrsn7\.vscode\extensions\bierner.markdown-mermaid-1.28.0\dist\index.js:1:1273)
>     at S.render (c:\Users\ehrrsn7\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\markdown-language-features\dist\extension.js:2:1506942)
>     at renderHTML (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\out\src\services\exporter\shared.js:34:40)
>     at renderPage (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\out\src\services\exporter\shared.js:19:16)
>     at PuppeteerExporter.exportFile (c:\Users\ehrrsn7\.vscode\extensions\jebbs.markdown-extended-1.1.4\out\src\services\exporter\puppeteer.js:51:44)
> ```
> **Solution**:\
> The issue was the `Foam` extension attempting to recreate obsidian features, including absolute paths for common images.
> Since these didn't work with the exporter, we converted these image paths to relative ones (generally ../../../..).
> The next step is to copy .vscode into each folder.