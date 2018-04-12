```graphviz
digraph finite_state_machine {
    rankdir=LR;
    "CI 3000" -> Verbundsteuerung -> Kühlstellenregler;
}
```

```graphviz
digraph finite_state_machine {
    rankdir=LR;
    size="8,5"

    node [shape = doublecircle]; S;
    node [shape = point ]; qi

    node [shape = circle];
    qi -> S;
    S  -> q1 [ label = "a" ];
    S  -> S  [ label = "a" ];
    q1 -> S  [ label = "a" ];
    q1 -> q2 [ label = "ddb" ];
    q2 -> q1 [ label = "b" ];
    q2 -> q2 [ label = "b" ];
}
```

# To begin with


Normaler Test

*Kursiver Text*

**Fett gedruckter Text**

~~Durchgestrichen~~


# Überschrift 1

## Überschrift 2

Tabelle

| Tables   |       Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is | left-aligned | $1600 |
| col 2 is | centered    |   $12 |
| col 3 is | right-aligned |    $1 |
&#124; 


    code

Syntax highlighted code:
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

```python
def foo():
    if not bar:
        return True```    
```


Ignore Markdown foramtting: \*our-new-project\* to \*our-old-project\*.


[Link to Google!](http://google.com)


# GitHub specials:

@mentionUserName

@octocat :+1: This PR looks great - it's ready to merge! :shipit:


# Other

Trennlinie

------

Trennlinie vorbei

1. First ordered list item
2. Another item
   * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
   1. Ordered sub-list
4. And another item.

![alt text](https://www.eckelmann.de/fileadmin/img/logo-eckelmann-ag.png "Ecekelmnan")


![Alt text](https://g.gravizo.com/source/custom_mark10?https%3A%2F%2Fraw.githubusercontent.com%2FTLmaK0%2Fgravizo%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
custom_mark10
  digraph G {
    size ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf};
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
custom_mark10
</details>


{% dot attack_plan.svg
    digraph G {
        rankdir=LR
        Earth [peripheries=2]
        Mars
        Earth -> Mars
    }
%}
