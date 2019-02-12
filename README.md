# gssh

Helps to SSH into gcloud instances:

- project fuzzy filter
- instance name fuzzy filter
- 1 day local project cache
- 5min local instance cache

#### install

```sh
$ brew install caarlos0/tap/gssh
```

You'll also need the `gcloud` cli available and set up, you can do so with:

```sh
$ brew cask install google-cloud-sdk
$ gcloud auth login
```

You may also need to change the default SSH username from `root` to something
else:

```sh
$ gssh --edit
```
