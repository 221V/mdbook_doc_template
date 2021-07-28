# Chapter 1

```
-module(test).
-compile([export_all, nowarn_export_all]).

test1(A) ->
  %A = 5,
  if A =:= 3 ->
      "333";
    A =:= 4 ->
      "444";
    A < 1 ->
      "010";
    A > 4 ->
      "505";
    true ->
      "777"
  end.

test2(A) ->
  %A = 5,
  case A of
    3 ->
      "333";
    4 ->
      "444";
    5.0 ->
      "010";
    5 ->
      "505";
    _ ->
      "777"
  end.
```
