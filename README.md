# tree-sitter-grammars

## Grammars

### Checkout

```shell
git submodule update --init
```

### Checkout recursively (for tests and etc.)

```shell
git submodule update --init --recursive
```

### Build

```shell
./make.py
```

Built artefacts are in `./output`

## Update

### Update sequence

```shell
git clone https://github.com/$USER/tree-sitter-grammars.git
git submodule init grammars/tree-sitter-$NAME/
git -C ./grammars/tree-sitter-$NAME/ checkout <commit>
git add ./grammars/tree-sitter-$NAME
git checkout -b feature/update-$NAME-grammar
git push
```
