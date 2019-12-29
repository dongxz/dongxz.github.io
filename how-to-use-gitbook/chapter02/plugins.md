# GitBook 插件



### 四、扩展插件



#### 4.3 代码块添加行号和复制按钮 code

[https://github.com/TGhoul/gitbook-plugin-code](https://github.com/TGhoul/gitbook-plugin-code)

```json
{
	"plugins": ["code"],
	"pluginsConfig": {
		"code": {
			"copyButtons": false
		}
	}
}
```

+ 显示代码行号，单行代码无行号
+ 复制按钮可关闭



#### 4.4 Todo 插件

[https://github.com/ly-tools/gitbook-plugin-todo](https://github.com/ly-tools/gitbook-plugin-todo)

```json
{
	"plugins": ["todo"]
}
```



#### 4.5 logo 定制

[https://github.com/matusnovak/gitbook-plugin-insert-logo](https://github.com/matusnovak/gitbook-plugin-insert-logo)

```json
{
	"plugins": ["insert-logo"],
	"pluginsConfig": {
		"insert-logo": {
			"url": "http://www.example.com/my-logo.png",
      "style": "background: none; max-height: 30px; min-height: 30px;"
		}
	}
}
```


#### 4.6 高级搜索 search-pro

支持中文搜索，在使用此插件之前，需要将默认的 `search` 和 `lunr` 插件去掉。

[https://github.com/gitbook-plugins/gitbook-plugin-search-pro](https://github.com/gitbook-plugins/gitbook-plugin-search-pro)

```json
{
	"plugins": [
		"-lunr", 
		"-search", 
		"search-pro"
	]
}
```



#### 4.7 emoji表情

[https://github.com/codeclou/gitbook-plugin-advanced-emoji](https://github.com/codeclou/gitbook-plugin-advanced-emoji)

```json
{
    "plugins": ["advanced-emoji"]
}
```



#### 4.8 Github图标

github 在右上角添加github图标。

[https://github.com/GitbookIO/plugin-github](https://github.com/GitbookIO/plugin-github)

```json
{
    "plugins": [ "github" ],
    "pluginsConfig": {
        "github": {
            "url": "https://github.com/your/repo"
        }
    }
}
```



#### 4.9 文字加底色

[https://github.com/GitbookIO/plugin-emphasize](https://github.com/GitbookIO/plugin-emphasize)

```json
{
    "plugins": ["emphasize"]
}
```



使用示例

```tex
This text is {% em %}highlighted !{% endem %}
This text is {% em %}highlighted with **markdown**!{% endem %}
This text is {% em type="green" %}highlighted in green!{% endem %}
This text is {% em type="red" %}highlighted in red!{% endem %}
This text is {% em color="#ff0000" %}highlighted with a custom color!{% endem %}
```



效果

![gitbook_plugin_emphasize.jpg](imgs/gitbook_plugin_emphasize.jpg)



#### 4.11 sharing-plus

[https://github.com/GitbookIO/plugin-sharing](https://github.com/GitbookIO/plugin-sharing)

```json
{
    "plugins": [
        "-sharing",
        "sharing-plus"
    ]
    "pluginsConfig": {
        "sharing": {
            "facebook": true,
            "twitter": true,
            "google": false,
            "weibo": false,
            "instapaper": false,
            "vk": false,
            "all": [
                "facebook", "google", "twitter", "weibo", "instapaper"
            ]
        }
    }
}
```


+ sharing配置中：true的代表直接显示在页面顶端，为false的不显示，不写默认为false
+ "all" 代表点击分享符号显示出来的所有分享按钮



