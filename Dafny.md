# Dafny

Dafny is a language which supports formal specification through pre-conditions, post-conditions, loop invariants and loop variants. A program/method is considered verified if the compiler can prove what changes are made through the conditions.

For example:

    method Add(a : int, b : int) returns (c : int)
    ensures c == a + b
    {
        c := a + b;
    }
Method *Add* returns the addition of the two parameters and proves this by including the post-condition *ensures c == a + b*.
