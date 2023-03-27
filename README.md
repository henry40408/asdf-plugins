# asdf-plugins

> :warning: All the plugins in this repository have been reviewed by me with my own eyes. Please use them with caution.

## What is the reason for creating this repository?

I wish to review and lock asdf plugins at a certain commit, but asdf does not offer such a feature.

- [Versioning of plugins #166](https://github.com/asdf-vm/asdf/issues/166)

## How do I use it?

First, you need to install [asdf](https://github.com/asdf-vm/asdf). Let's assume it is installed in `~/.asdf`.

```bash
$ cd ~/.asdf
$ mv plugins plugins.old # If you already have any plugins installed,
$ git clone https://github.com/henry40408/asdf-plugins.git --branch plugins plugins
$ git checkout [commit] # I strongly recommend that you select a commit and check out from this repository.
$ git submodule init
$ git submodule update
```
That's all.

## Why do you place the plugins in another branch called "plugins"?

asdf does not exclude files such as `LICENSE.txt` and `README.md` from plugins. Therefore, when we run a command such as `asdf reshim`, an error like the following may occur:

```
No such plugin: LICENSE.txt
```

## License

MIT
