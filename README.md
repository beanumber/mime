# mime

[![Build Status](https://travis-ci.org/yihui/mime.svg)](https://travis-ci.org/yihui/mime)

This is an R package for mapping filename extensions to [MIME
types](http://en.wikipedia.org/wiki/Internet_media_type), based on the data
[derived](R/mime.R) from `/etc/mime.types`.

```r
# installation
install.packages('mime', repos = 'https://cran.rstudio.com')

library(mime)
guess_type(c('a/b/c.html', 'd.pdf', 'e.odt', 'foo.docx', 'tex'))
# [1] "text/html"                                                              
# [2] "application/pdf"                                                        
# [3] "application/vnd.oasis.opendocument.text"                                
# [4] "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
# [5] "text/x-tex"
```
