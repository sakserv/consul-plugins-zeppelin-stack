Zeppelin Stack Consul Plugin
----------------------------
This plugin is a post task used to install the Apache Zeppelin stack via Cloudbreak provisioned clusters.

To add the recipe, execute the following via cloudbreak-shell
```
recipe add --url https://raw.githubusercontent.com/sakserv/consul-plugins-spark-shuffle/master/zeppelin-stack.json
```

Get the recipe id
```
recipe list
```

Add the recipe to the hostgroup that runs the Ambari server
```
hostgroup configure --hostgroup host_group_client_1 --recipeIds 217
```
