```shell
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo tee /usr/share/keyrings/yarn-archive-keyring.gpg >/dev/null
```

```shell
echo "deb [signed-by=/usr/share/keyrings/yarn-archive-keyring.gpg] https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
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
