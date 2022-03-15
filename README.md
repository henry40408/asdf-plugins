# asdf-repository

> :warning: All plugins in this repository are reviewed by my bare eyes. Use with caution.

## How to Use?

First, install [asdf](https://github.com/asdf-vm/asdf). Let's assume it is installed on `~/.asdf`.

```bash
cd ~/.asdf
mv plugins plugins.old # if you already have any plugins installed
git clone https://github.com/henry40408/asdf-plugins.git plugins
git checkout [commit] # I strongly suggest you pick a commit and checkout
git submodule init
git submodule update
```

That's all.

## License

MIT
