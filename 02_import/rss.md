---
title: RSS
---

To import your posts from an RSS feed (local or remote), run:

{% highlight bash %}
$ ruby -rubygems -e 'require "jekyll-import";
    JekyllImport::Importers::RSS.run({
      "source" => "my_file.xml"
    })'
{% endhighlight %}

The `source` field is required and can be either a local file or a remote one.
