# gssh

Helps to SSH into gcloud instances:

- project fuzzy filter
- instance name fuzzy filter
- 1 day local project cache
- 1 hour local instance cache

#### install

```sh
brew install caarlos0/tap/gssh
```

You'll also need the `gcloud` cli available and set up, you can do so with:

```sh
brew cask install google-cloud-sdk
gcloud auth login
```

#### usage

**Basic usage:**

```sh
gssh
```

**Pre-filter project:**

```sh
gssh my-proj
```

**Pre-filter both project and instance:**

```sh
gssh my-proj instance-xyz
```

**Flush caches:**

```sh
gssh --flush
```

**Port-forward instance port 9200 to localhost:19200:**

```sh
GSSH_FLAGS='-L 19200:localhost:9200' gssh my-proj elasticsearch
```
