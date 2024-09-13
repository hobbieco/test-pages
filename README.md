# test-pages
test react and vite with github pages

- URL : https://{ACCOUNT}.github.io/{REPO_NAME}
```shell
yarn create vite {path} [--template react-swc-ts]
cd {path}
yarn install
yarn add gh-pages --save-dev
```
- edit package.json
```json
"homepage": "htpps://{ACCOUNT}.github.io/{REPO_NAME}",
"scripts": {
  ...
  "predeploy": "yarn build",
  "deploy": "gh-pages -d dist"
}
```

- run react
```shell
yarn dev
```

- deploy gh-pages
```shell
yarn deploy
```

- github setting
  - repository settings > pages > branch
    - gh-pages and root

# SCSS

- need python module distutils
```shell
brew install python-setuptools
# or
python3 -m pip install setuptools
```

- install node module
```shell
yarn add -D sass-embedded
```

- rename css file to scss
```shell
mv index.css index.scss
mv App.css App.scss
```