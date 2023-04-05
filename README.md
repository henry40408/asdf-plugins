# asdf-plugins

[![License](https://img.shields.io/github/license/henry40408/asdf-plugins)](https://github.com/henry40408/asdf-plugins/blob/main/LICENSE)

> :warning: All the plugins in this repository have been reviewed by me personally. Please use them with caution.

## What is the reason behind the creation of this repository?

I would like to review and lock asdf plugins at a specific commit, but asdf does not provide such a feature.

- [Versioning of plugins #166](https://github.com/asdf-vm/asdf/issues/166)

## How should I use it?

First, you need to install [asdf](https://github.com/asdf-vm/asdf). Let's assume it has been installed in `~/.asdf`.

```bash
$ cd ~/.asdf
$ mv plugins plugins.old # If you already have any plugins installed,
$ git clone https://github.com/henry40408/asdf-plugins.git --branch plugins plugins
$ git checkout [commit] # I strongly recommend selecting a commit and checking out from this repository.
$ git submodule init
$ git submodule update
```

That's all.

## Why do you place the plugins in a separate branch named `plugins`?

asdf does not exclude files such as `LICENSE.txt` and `README.md` from plugins. Therefore, when running a command such as asdf reshim, an error like the following may occur:

```
No such plugin: LICENSE.txt
```

## License

MIT
