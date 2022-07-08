# lazyppl Pandoc / bootstrap

To generate a webpage from Literate Haskell, use a command like:

```bash
pandoc -f markdown+lhs -s WienerDemo.lhs -t html -o Wiener.html --template=lazyppltemplate.html
```

For example, to deal with all Literate Haskell files:

```bash
for f in *.lhs; do pandoc -f markdown+lhs -s "${f%.*}.lhs" -t html -o "${f%.*}.html" --template=lazyppltemplate.html ; done
```

# lazyppl source

The source code along with build instructions can be found in the `lazyppl` directory.
