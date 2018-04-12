


<p align="center">
    <img alt="Alt Text" src="https://g.gravizo.com/source/custom_mark11?https%3A%2F%2Fgithub.com%2FMarkusMuellerMM%2Ftestmarkdown20180412%2Fedit%2Fmaster%2Ftest2.md" />
</p>


![Alt text](https://g.gravizo.com/svg?
  digraph G {
    aize ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf}
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
)

![Alt text](https://g.gravizo.com/source/custom_mark11?https%3A%2F%2Fgithub.com%2FMarkusMuellerMM%2Ftestmarkdown20180412%2Fedit%2Fmaster%2Ftest2.md)

<details> 
<summary></summary>
custom_mark11
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
custom_mark11
</details>


{% dot output.png
	digraph G {
		rankdir=LR
		S0 -> A [label="-"]
		A -> B [label="-"]
		A -> C [label=">"]

		A [peripheries=2]
		B [peripheries=2]
		C [peripheries=2]
	}
%}
