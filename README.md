```shell
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/yarn-archive-keyring.gpg
```

```shell
gpg --no-default-keyring --keyring /usr/share/keyrings/yarn-archive-keyring.gpg --list-keys
```

```shell
sudo apt update && sudo apt install yarn
```

```shell
echo 'export PATH="$HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH"' >> ~/.bashrc && source ~/.bashrc
```

```shell
yarn --version
```
