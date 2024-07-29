# learn-rbenv-100

|本期版本|上期版本
|:---:|:---:
`Mon Jul 29 14:38:24 CST 2024` | -

## rbenv-doctor

```
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/HEAD/bin/rbenv-doctor | bash
```

## ruby-build

> [Suggested build environment](https://github.com/rbenv/ruby-build/wiki#suggested-build-environment)

```bash
export RUBY_CONFIGURE_OPTS="--disable-install-doc --disable-install-rdoc"
```


```bash
set -Ux RUBY_CONFIGURE_OPTS --disable-install-doc --disable-install-rdoc \
	--with-openssl-dir=(brew --prefix openssl@1.1)
```

## Fish

> `~/.config/fish/config.fish`

```bash
rbenv init - --no-rehash fish | source
```

**XQuartz**

```bash
if which rbenv > /dev/null
    rbenv init - fish | source
end
```


## Ref

* <https://github.com/rbenv/rbenv>、<https://github.com/rbenv/rbenv-installer>
* <https://github.com/rbenv/ruby-build>
* <https://github.com/AndorChen/rbenv-china-mirror>
* <https://github.com/rbenv/rbenv-vars>
* [How to automate rbenv installations](https://relativkreativ.at/articles/how-to-automate-rbenv-installations)