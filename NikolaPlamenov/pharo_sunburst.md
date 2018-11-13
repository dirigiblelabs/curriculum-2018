# Sunburst diagram source code
##### Date:2018-11-13_15-51-25
##### Author: npd

## Dependencies

* Roassal

## View the pre-built plot

Download the [graphics library][roassal] and [HTML root file][sunburst].

## Raw source code

```
| p b data webide appserver lb |
webide := Array new: 7.
webide at: 1 put: 'Layouting' -> (Array with: 'GoldenLayout');
        at: 2 put: 'Perspectives';
        at: 3 put: 'Views';
        at: 4 put: 'Events';
        at: 5 put: 'Forms' -> (Array with: 'Angular');
        at: 6 put: 'Editors' -> (Array with: 'Orion' with: 'Ace' with: 'Monaco');
        at: 7 put: 'Theming' -> (Array with: 'Bootstrap').

appserver := Array new: 16.
appserver at: 1 put: 'JavaScript Engine' -> (Array with: 'Rhino' with: 'Nashorn' with: 'V8');
            at: 2 put: 'Web' -> (Array with: 'Built-in');
            at: 3 put: 'Wiki Engine' -> (Array with: 'Mylyn');
            at: 4 put: 'Indexing' -> (Array with: 'Lucene');
            at: 5 put: 'Repository';
            at: 6 put: 'Extensions';
            at: 7 put: 'Persistence';
            at: 8 put: 'Security';
            at: 9 put: 'Configuration';
            at: 10 put: 'Scheduler';
            at: 11 put: 'Publisher';
            at: 12 put: 'Job Engine' -> (Array with: 'Quartz');
            at: 13 put: 'Messaging' -> (Array with: 'ActiveMQ');
            at: 14 put: 'Processes' -> (Array with: 'Flowable');
            at: 15 put: 'Templating' -> (Array with: 'Mustache');
            at: 16 put: 'Documents' -> (Array with: 'Chemistry').

data := Array new: 2.
data at: 1 put: 'Web IDE' -> webide.
data at: 2 put: 'App Server' -> appserver.

p := RTPalette c4.

b := RTSunburstBuilder new.
b layout sunburstWithRadius: 300.
b shape
    color: [ :o |
        o class == Association
            ifTrue: [ p second ]
            ifFalse: [ p third ] ].
b
    leafColor: p first;
    explore: data
    using: [ :o |
        o class == Association
            ifTrue: [ o value ]
            ifFalse: [ o isString
                    ifTrue: [ #() ]
                    ifFalse: [ o ] ] ].
b build.
lb := RTLegendBuilder new.
lb view: b view.
lb addText: 'Depending on the target cloud platform, in Eclipse Dirigible can be integrated the services provided by the underlying platform.';
    addText: 'File System';
    addText: 'NoSQL';
    addText: 'Database';
    addText: 'IDM';
    addText: '...'.
lb build.
b view.
```

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [roassal]: <roassal.js>
   [sunburst]: <dirigible_sunburst.html>
