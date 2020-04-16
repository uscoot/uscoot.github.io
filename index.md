
## Welcome to My Blog

You can use the [editor on GitHub](https://github.com/uscoot/uscoot.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
提莫队长
### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/uscoot/uscoot.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

**请求URL：** 
- ` /tv-delivery-fee-template-entity/queryDeltemp `
  
**请求方式：**
- POST 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|goodsGroupId |是  |Integer |商品组id  |
|country |是  |String | 城市    |
|regions     |是  |String | 地区   |
|goodsId     |是  |Integer | 商品id   |
|num     |是  |Integer | 数量  |

 **返回示例**

``` 
{
    "code": 200,
    "msg": "处理成功!",
    "data": {
        "resultmap": [
            {
                "deliveryFee": 600,
                "venderId": 1015,
                "deliveryType": 1,
                "destination": "{\"country\":\"AF\",\"regions\":\"BGL,BAL,BAM\",\"id\":\"_trackId11\"}",
                "templateFeeId": 22,
                "estimatedDuration": "3"
            },
            {
                "deliveryFee": 800,
                "venderId": 1015,
                "deliveryType": 2,
                "destination": "{\"country\":\"AF\",\"regions\":\"BGL,BDG,BDS\",\"id\":\"_trackId13\"}",
                "templateFeeId": 23,
                "estimatedDuration": "5"
            }
        ]
    }
}

所选地区暂不配送：
{
    "code": 500,
    "msg": "Out of delivery !",
    "data": {}
}
```