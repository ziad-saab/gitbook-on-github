# Chapter exercise

Exercises format

An exercise is defined by 4 simple parts:

- Exercise Message/Goals (in markdown/text)
- Initial code to show to the user, providing a starting point
- Solution code, being a correct solution to the exercise
- Validation code that tests the correctness of the user's input

{% exercise %}
Define a variable `x` equal to 10.
{% initial %}
var x =
{% solution %}
var x = 10;
{% validation %}
assert(x == 10);
{% context %}
// This is context code available everywhere
// The user will be able to call magicFunc in his code
function magicFunc() {
    return 3;
}
{% endexercise %}