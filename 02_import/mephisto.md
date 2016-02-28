---
title: Mephisto
---

To import your posts from [Mephisto](http://www.mephistoblog.com), run:

{% highlight bash %}
$ ruby -rubygems -e 'require "jekyll-import";
    JekyllImport::Importers::Mephisto.run({
      "dbname"   => "name",
      "user"     => "myuser",
      "password" => "mypassword",
      "host"     => "myhost"
    })'
{% endhighlight %}

The only required fields are `dbname` and `user`. `password` defaults to `""`
and `host` defaults to `"localhost"`.