---
title: Joomla 3
---

To import your posts from a [Joomla 3](http://joomla.org) installation, run:

{% highlight bash %}
$ ruby -rubygems -e 'require "jekyll-import";
    JekyllImport::Importers::Joomla.run({
      "dbname"   => "name",
      "user"     => "myuser",
      "password" => "mypassword",
      "host"     => "myhost",
      "category" => "category",
      "prefix"   => "mytableprefix"
    })'
{% endhighlight %}

The only required fields are `dbname`, `prefix` and `user`. `password` defaults to `""`,
and `host` defaults to `"localhost"`.

If the `category` field is not filled, all articles will be imported, except the ones that are 
uncategorized. 
