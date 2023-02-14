**Software Architecture in Practice** Third Edition 软件构架实践（第三版）
===

- Len Bass （林·巴斯） 

- Paul Clements （保罗·克莱门茨） 
- Rick Kazman （瑞克·凯兹曼）

_中文由机器翻译，主要依赖[Google翻译](https://translate.google.com)，在明显的错误处作了简单地调整。_

_如有copyright问题，请联系。_

# How to
We are using gitbook to organize this book and hosted the output on github [https://suseme.github.io/sw_arch_in_p]().
## How to build
```bash
# Generate HTML pages
docker run -v $PWD:/srv/gitbook -v $PWD/docs:/srv/html fellah/gitbook gitbook build . /srv/html
# Generate PDF file
docker run -v $PWD:/srv/gitbook -v $PWD/docs:/srv/html fellah/gitbook gitbook pdf . /srv/html/sw_arch_in_p.pdf
# Generate EPub format
docker run -v $PWD:/srv/gitbook -v $PWD/docs:/srv/html fellah/gitbook gitbook epub . /srv/html/sw_arch_in_p.epub
# Generate Mobi format
docker run -v $PWD:/srv/gitbook -v $PWD/docs:/srv/html fellah/gitbook gitbook mobi . /srv/html/sw_arch_in_p.mobi
```

## How to run gitbook server
```bash
docker run -p 4000:4000 -v $PWD:/srv/gitbook -v $PWD/docs:/srv/gitbook/_book fellah/gitbook gitbook serve ./
```
