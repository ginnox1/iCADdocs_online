To use Github-friendly Markdown (gfm), we can use:

pandoc --extract-media=. -s mydoc.docx -t gfm -o mddoc.md

