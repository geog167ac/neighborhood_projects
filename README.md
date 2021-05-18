# neighborhood_projects
1. Follow the guide on how to properly setup your ruby enviroment before installing jekyll.
2. Project uses jekyll to power the website.
3. In order to install jekyll, follow the jekyll official documentation.
4. I'm using rvm to manage ruby version and gems
5. After running `gem install jekyll` I ran into the following error
`In file included from binder.cpp:20:
./project.h:119:10: fatal error: 'openssl/ssl.h' file not found
#include <openssl/ssl.h>` 
6. To fix the issue read this post - https://github.com/eventmachine/eventmachine/issues/932
7. Solution - Before running `gem install jekyll` run `gem install eventmachine -- --with-openssl-dir=/usr/local/opt/openssl@1.1` and then run `gem install jekyll`
8. Jekyll installed.