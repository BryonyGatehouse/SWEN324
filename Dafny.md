# Dafny

Dafny is a language which supports formal specification through pre-conditions, post-conditions, loop invariants and loop variants. A program/method is considered verified if the compiler can prove what changes are made through the conditions.

For example:

    function Positive(a : int) : int
    {
        if a < 0 then -a
        else a
    }

    lemma check(a : int)
        ensures Positive(a) >= 0
        ensures if a < 0 then Positive(a) == -a else Positive(a) == a
        ensures if a < 0 then Positive(a) != a else Positive(a) == a
        ensures if a == 0 then Positive(a) == 0 else Positive(a) > 0
        {}
Method *Positive* returns the positive version of the given integer. The lemma *check* confirms that it performs the expected task:
- Checks that the result is always positive
- Checks that if the integer is negative its positive value is returned
- Checks that if the integer is negative the returned value is not the same as the integer
- Checks that if the integer is 0, the returned value is 0
