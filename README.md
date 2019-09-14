# hexo-github-card-customize
从`hexo-github-card`fork而来, 增加了一些默认值配置

[hexo-github-card](https://github.com/Gisonrg/hexo-github-card).


## Install

NPM
```
npm install --save hexo-github-card-customize
```

Yarn
```
yarn add hexo-github-card-customize
```

## Usage

Insert `githubCard` tag in your article:

```
{% githubCard user:your_user [repo:your_repo] [width:400] [height:200] [theme:default] [client_id:your_client_id] [client_secret:your_client_secret] [align:text-align_position] %}
```

Argument | Description
-------- | -----------
user     | GitHub user name
repo     |  (Optional) GitHub repository name of the user. If omit then display only the user profile
height   | (Optional) Widget's height (in 'px'). Default is 200.
width   | (Optional) Widget's width (in 'px'). Default is 400.
client_id | (Optional) Your GitHub app client_id
client_secret | (Optional) Your GitHub app client_secret
align | (Optional) What kind of text-align is you want. Default is center.

(Configuration are consistent with [github-cards](https://github.com/lepture/github-cards#widgetjs))

Example:

Display user profile only
```
{% githubCard user:Gisonrg %}
```

Display a repo
```
{% githubCard user:Gisonrg repo:hexo-github-card %}
```
edit `_config.yml`
```yaml
# _config.yml
github_card:
  width: 100%
  height: 200px
  theme: default
  align: center
  target: blank
```

License
=======

[MIT](LICENSE)
