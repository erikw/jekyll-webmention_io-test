# jekyll-webmention_io-test
Basic Jekyll webmentions test site deployed at https://jekyll-webmention-io-test.netlify.app/

Sending webmentions with
```console
$ bundle exec jekyll webmention
```
does not work. Do manually instead

```console
$ curl -si https://webmention.io/jekyll-webmention-io-test.netlify.app/webmention \
  -d source=https://jekyll-webmention-io-test.netlify.app/update/2021/07/12/test-post.html \
  -d target=https://erikw.me/blog/tech/open-sourcing-my-second-jekyll-plugin-gossary-tooltip/
```
