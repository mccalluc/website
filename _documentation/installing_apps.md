---
layout: documentation
title:  Installing Applications
permalink: /documentation/installing_apps
---

{% include todo.html %}

* Replace content with how to install a binary description


## OLD CONTENT

Note: Please ignore this part if you want to set up a dev environment.

{% highlight bash  %}
git clone https://github.com/Caleydo/caleydo_web_container.git
cd caleydo_web_container
vagrant up
# wait and get some coffee. this will take a while
vagrant sshinstallation.mdinstallation.md
{% endhighlight %}


{% highlight bash  %}
# 1a clone the repositories and their dependencies
./manage.sh clone demo_app
./manage.sh clone caleydo_server

# OR 1b install the latest published plugin
./manage.sh install demo_app
./manage.sh install caleydo_server

# 2 resolve dependencies of plugins
./manage.sh resolve

# 3 start caleydo web
./manage.sh server
{% endhighlight %}

Access: http://localhost:9000 or http://192.168.50.52:9000 and have fun :)

Note:
Depending whether you installed the python server `caleydo_server` or the Javascript server `caleydo_server_js`, call the corresponing grunt task: `server` and `server_js`.

TODO: add list of applications (dynamically generated?)

[List of Sample Applications](https://github.com/Caleydo/?utf8=%E2%9C%93&query=sample)