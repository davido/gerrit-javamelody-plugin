Gerrit Javamelody plugin allows to monitor Gerrit server.

It integrates JavaMelody [1] in Gerrit in order to retrieve live
instrumentation data from Gerrit.

When plugin is deployed, Monitoring top menu is available for members of the
Administrators group.

Howto build:

This plugin is built with Buck, like Gerrit itself.

Clone or link this plugin to the plugins directory of Gerrit tree
and issue the command:

```
  buck build plugins/javamelody:javamelody
```

The output is created in

```
  buck-out/gen/plugins/javamelody/javamelody.jar
```

This project can be imported into the Eclipse IDE:

```
  ./tools/eclipse/project.py
```

* [1] https://code.google.com/p/javamelody
