---
deck: info
---


<!-- basicblock-start oid="ObsyhKXCfujLHd3hnaWm9cjm" -->
Prop. `List` module::
- `List.init -> int -> (int->'a) -> 'a list`
- `List.lentgh -> 'a list -> int`
- `List.mem -> 'a -> 'a list -> bool`
- `List.for_all -> ('a -> bool) -> 'a list -> bool`
- `List.exists -> ('a -> bool) -> 'a list -> bool`
- `List.rev -> 'a list -> 'a list`
- `List.iter -> ('a -> ()) -> 'a list -> ()`
- `List.map -> ('a -> 'b) -> 'a list -> 'b list`
- `List.filter -> ('a -> bool) -> 'a list -> 'a list`
- `List.partition -> ('a -> bool) -> 'a list -> 'a list * 'a list`
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsRPuO08G2lgeyLMbeDG7TF" -->
Prop. `Array` module::
- `Array.init -> int -> (int->'a) -> 'a array`
- `Array.length -> 'a array -> int`
- `Array.iter -> ('a -> ()) -> 'a array -> ()`
- `Array.iteri -> (int -> 'a -> ()) -> 'a array -> 'b array`
- `Array.map -> ('a -> 'b) -> 'a array -> 'b array`
- access: `ar.(i)`
- modify: `ar.(i) <- v`.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsBSahXtoFWFgTDibw1qZKF" -->
Prop. `Random` module::
- `Random.self_init -> () -> ()`
- `Random.init -> int -> ()`
- `Random.bool -> () -> bool`
- `Random.int -> int -> int`
- `Random.float -> float -> float`
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs7Eydssyms1ZynUAtYAf7I" -->
Prop. ref in Ocaml::
- define: `let a = ref b`
- access: `!a`
- modify: `a:=x;`
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsjRdE9AIfgNGQfXvtUEKGT" -->
Prop. loops in Ocaml::
- for: `for i=k to n do ... done;`
- for: `for i=k downto n do ... done;`
- while: `while cond do ... done;`
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsreyXHG9l2hD1chrtfcwO7" -->
Prop. exception in Ocaml::
- define: `exception MyException;;`
- raise: `raise MyException`
- try/catch: `try expr with |MyException->expr`
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsogTGarkxPeUa83CIiOSSe" -->
Prop. match pattern in Ocaml::
- declaring: `match expr with`
- basic case: `| pattern -> expr`
- conditional: `| pattern when guard -> expr`
- binding: `| pattern as x -> expr`
- pattern union: `| pattern1 | pattern2 -> expr`
- default: `| _ -> expr`
- Variant: `| Pair (x,y) -> expr`
- Record: `| {hey=x; _} -> expr`
- list: `| h::t -> expr`
<!-- basicblock-end -->


