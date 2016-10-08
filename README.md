
2016 프로그래밍 언어 과제
----

## Link

* [과목 페이지](https://github.com/snu-sf-class/pl201602)
* [교과서](http://www.cis.upenn.edu/~bcpierce/sf/current/index.html)
* 참조: [tutorial-nahas](http://kr.archive.ubuntu.com/ubuntu)

## 일정


| Due          | Due (Delay)  | Description  | Points |
| ------------ | ------------ | ------------ | ------ |
| Oct.3 23:59  | Oct.10 23:59 | Assignment 1 | 50     |
| Oct.10 23:59 | Oct.17 23:59 | Assignment 2 | 100    |



## 요약

* Every coq command ends with a period.
* The **goal** is the theorem we're trying to prove.
* A **subgoal** is what we are trying to prove at any point during the proof.
* A **prop** is not either true false. A **prop** either has a proof or it does not have proof.

## Grammer

### vernacular

The vernacular language manages definitions, and each of its commands starts widh a capital letter: `Theorem`, `Proof`, and `Qed`.

#### Theorem

* Instead of `Theorem`, you may also see proofs that start with `Lemma`, `Remark`, `Fact`, `Corollary`, `Proposition`, which all mean the ***SAME*** thing. 

#### QED

* Instead of `Qed`, you may also see proofs that end widh `Admitted` or `Defined`, but these mean ***DIFFERENT*** things.

#### Inductive

* `Inductive` lets you create a new type.

### tactics

The tactics language is used to write proofs, and its commands start with a lower-case letter: `intros`, and `exact`.

#### intros

* `intros A` means "assume A".


* If the subgoal starts with `(forall <name> : <type>, ...)` then use tactic `intros <name>`.

* If the subgoal starts with `<type> -> … ` then use tactic `intros <name>`.

  ​

#### exact

* If the subgoal matches an hypothesis, then use tactic `exact <hyp_name>`.

#### pose

* If you have an hypothesis `<hyp_name>: <type1> -> <type2> -> … -> <result_type>` or an hypothesis `<hyp_name>: (forall <obj1>: <type1> , forall (<obj2>: <type2>, … <result_type> …))` or any combination of `->`, `and`, `forall`, and you have hypotheses of type `type1`, `type2`, … , then use tactic `pose` to create something of `result_type`.
* `pose (A := B C)` computes **A** that is associated with **B** and **C**.

### Gallina

The Gallina language is used to express what you want to prove, and its expression use lots of operators and parentheses: `(forall A: Prop, A -> A)`.



## Proof

### Proof going forward

* `pose`

### Proof going backward

#### small

#### large

#### huge

