### 1.npm仓库设置

修改默认仓库

```bash
npm config set registry http://registry.npm.taobao.org/
```

原始仓库

npm config set registry https://registry.npmjs.org/

```bash
npm config set registry http://registry.npm.taobao.org/
```

安装cnpm

```bash
npm install -g cnpm --registry=https://registry.npmmirror.com
```

或

```bash
alias cnpm="npm --registry=https://registry.npmmirror.com \
--cache=$HOME/.npm/.cache/cnpm \
--disturl=https://npmmirror.com/dist \
--userconfig=$HOME/.cnpmrc"

# Or alias it in .bashrc or .zshrc
$ echo '\n#alias for cnpm\nalias cnpm="npm --registry=https://registry.npmmirror.com \
  --cache=$HOME/.npm/.cache/cnpm \
  --disturl=https://npmmirror.com/dist \
  --userconfig=$HOME/.cnpmrc"' >> ~/.zshrc && source ~/.zshrc
```

[淘宝 NPM 镜像 (npmmirror.com)](https://npmmirror.com/)