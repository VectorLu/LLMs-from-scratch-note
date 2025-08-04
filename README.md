# Note for LLM-from-scratch

Build my own LLM from scratch.

## repo info

Note for learn [LLM-from-scratch](https://github.com/rasbt/LLMs-from-scratch#)

中文项目参考：[LLMs-from-scratch-CN](https://github.com/MLNLP-World/LLMs-from-scratch-CN)

由于这个中文项目没有更新，所以还是以原项目为主。我尽量每月与原项目保持同步更新。



整个 repo 采用 git submodule 来管理原项目、衍生的中文项目，和我自己学习实践的经验。使用 git submodule 是为了与上游项目（主要是原项目）保持同步更新。这样即使我没有更新，你下载项目后，也可以通过 `git submodule update --remote` 来更新。这是 [LLMs-from-scratch-CN](https://github.com/MLNLP-World/LLMs-from-scratch-CN) 没有做到的。

## how to use this repo

由于使用了 submodule，所以需要使用如下命令下载这个 repo，好处是可以同时下载原项目和中文项目，不用再单独下载。

```bash
git clone --recurse-submodules https://github.com/VectorLu/LLMs-from-scratch-note
```

> [!NOTE] If you already use simple `git clone` to clone the project and forgot `--recurse-submodules`, you can combine the `git submodule init` and `git submodule update` steps by running `git submodule update --init`. To also initialize, fetch and checkout any nested submodules, you can use the foolproof `git submodule update --init --recursive`.

> [!NOTE] 如果你已经克隆了项目并且忘记了 `--recurse-submodules` ，你可以通过运行 `git submodule update --init` 来结合 `git submodule init` 和 `git submodule update` 步骤。要同时初始化、获取并检出任何嵌套的 submodule，你可以使用万无一失的 `git submodule update --init --recursive` 。


## how to update this repo

```bash
# 更新主项目
git pull

# 更新 submodule
git submodule update --remote
```


