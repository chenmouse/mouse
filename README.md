## 陈泽昊

You can use the [editor on GitHub](https://github.com/chenmouse/mouse/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### I AM DREAMING

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# RStudio图片插入实验(从RStudio端口编辑)
library(jpeg)
library(reshape2)
img<-readJPEG("test.jpg")
dim(img)
longImage <- melt(img)
rgbImage <- reshape(longImage, timevar='Var3',idvar=c('Var1','Var2'), direction='wide')
head(rgbImage)
colorColumns<- rgbImage[, substr(colnames(rgbImage), 1, 5)== "value"]
dev.new()
with(rgbImage,plot(Var2, Var1, col = rgb(colorColumns), asp = 1, pch =".",axes=T,xlab='',ylab=''))

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```
[图片来源：观察者网](https://www.bilibili.com/video/BV1Dk4y1R7AL)

![Image](https://github.com/chenmouse/mouse/blob/master/Picture/test.jpg)

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

额外注释：上传图片如果不显示可前往[CSDN](https://blog.csdn.net/qq_38232598/article/details/91346392)查找办法

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/chenmouse/mouse/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
