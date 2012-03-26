# HTTP Footer filter module for Nginx

## Introduction

This is a module that is distributed with
[tengine](http://tengine.taobao.org) which is a distribution of
[Nginx](http://nginx.org) that is used by the e-commerce/auction site
[Taobao.com](http://en.wikipedia.org/wiki/Taobao). This distribution
contains some modules that are new on the Nginx scene. The
`ngx_http_footer_filter` module is one of them.

This module implements a body filter that adds a given string to the
page footer.

You might say that it provides a particular case of the
[http sub module](http://wiki.nginx.org/HttpSubModule) in the sense
that it adds something to the footer. You can do the same using the
`http sub module` but using the footer filter should be faster since
there's no string matching done on the request body.

## New Repository

The new repo is at
[https://github.com/taobao/nginx-http-footer-filter](https://github.com/taobao/nginx-http-footer-filter).
