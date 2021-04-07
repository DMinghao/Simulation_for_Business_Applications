
Let $G$ = ($V$, $E$, $C$) be a directed acyclic multigraph that denotes the system's process flow (A multigraph is a graph that allows more than one edges to have the same endpoint)

Let $V$ denotes a set of vertices, where $V \ni \{v_1, v_2, ... , v_n\}$ 

Let $v_s$ denotes the source vertex $v_t$ denotes the target vertex in a flow, and $s \lt t$

Let $E$ denotes a set of edges, where  $E \subseteq \{(v_s,v_t)\mid v_s,v_t\in V\}$ and $\forall e \in E \mid (e_{(v_s, v_t)}=e_{(v_a, v_b)}) \iff (v_s = v_a \land v_t = v_b)$

Let $C$ be a set of non-negative capacity functions, i.e. $c : V \times V \rightarrow \R_{\infin}$ or $c : E \rightarrow \R_{\infin}$, where $\forall e \in E \: \exist ! \: c(e_{(v_s, v_t)}) \implies f:E\rightarrow C$

Bottleneck := $\exist e \in E \mid c(e_{(v_s, v_t)}) = \min\limits_{x\in E} f(x)$

Consider Question A's situation: 

System $G$ = ($V$, $E$, $C$)

$V = \{v_1, v_2, v_3, v_4, v_5\}$

$E = \{e_{(v_1, v_2)}, e_{(v_2, v_3)}, e_{(v_3, v_4)}, e_{(v_4, v_5)}\}$

$c(e) = 60 / 10 = 6 \: units/hr$

$C = \{c(e_{(v_1, v_2)}), c(e_{(v_2, v_3)}), c(e_{(v_3, v_4)}), c(e_{(v_4, v_5)})\} = \{6, 6, 6, 6 \}$

$\because \min\limits_{x\in E} f(x) = 6$

$\therefore \forall e \in E \mid c(e) = \min\limits_{x\in E} f(x)$

$\therefore$ All four stations are the Question A system's bottleneck
