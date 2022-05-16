# asdf-repository

> :warning: All plugins in this repository are reviewed by my bare eyes. Use with caution.

## Why create this repository?

I want to review and lock asdf plugins at certain commit and asdf does not provide such feature:

- [Versioning of plugins #166](https://github.com/asdf-vm/asdf/issues/166)

## How to Use?

First, install [asdf](https://github.com/asdf-vm/asdf). Let's assume it is installed on `~/.asdf`.

```bash
$ cd ~/.asdf
$ mv plugins plugins.old # if you already have any plugins installed
$ git clone https://github.com/henry40408/asdf-plugins.git --branch plugins plugins
$ git checkout [commit] # I strongly suggest you pick a commit and checkout from this repository
$ git submodule init
$ git submodule update
```
That's all.

## Why do you put plugins in branch named plugins?

asdf doesn't exclude files like `LICENSE.txt` and `README.md` from plugins, so when we run command such as `asdf reshim`, an error like the following occurs:
```
No such plugin: LICENSE.txt
```
## License

MIT
