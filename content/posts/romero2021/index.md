+++
title = "Romero2021"
author = ["Romero", "Julien"]
date = 2025-01-07T13:58:00+01:00
draft = false
+++

## Pyformlang: An Educational Library for Formal Language Manipulation {#pyformlang-an-educational-library-for-formal-language-manipulation}

The author of this paper propose pyformlang, an alternative to JFLAP, wrote in python3
instead of Java. The main idea of this work is to give students a tool that aims
to help them with formal language representation. To commit this task, the
author has used the algorithms proposed by Hopcroft in _Automata Theory,
Languages and Computatiuon_

This tools is not a fully alternative to JFAP, as, in this case, the library
proposes a Domaine Specific Language (DSL), while JFLAP is a fully graphical
tool to interact with formal languages. Also, there are some differences between
both implementation. In Pyformlang, the author wanted to make it more general
and easy to use, allowing special case in regex definition. Usually, the
alphabet consists of all single characters (minus special ones), thus creating a
concatenation when encountering consecutive characters. In Pyformlang, they
considered that consecutive characters are a single symbol. So the tool has a
more general approach not bound to text processing.
