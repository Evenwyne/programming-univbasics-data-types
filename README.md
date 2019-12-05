# Data Types

## Learning Goals

* Define "reserved word"
* Define data versus other words in a Ruby file
* Describe what a data type is
* Identify an `Integer`
* Identify a `Float`
* Identify Boolean Values
* Identify `String` Values
* Identify `Symbol` Values
* Name the Scalar Data Types in Ruby
* Ask IRB for the Data Type of a Value

## Introduction

Thus far in all the _expression_ we've learned, we've only used one type of
data in our constant expressions: numbers. To be more specific, we've only used
_whole_ numbers, or "Integers." But the world is not simply Integers, there are
other things in the world: text, truth and falsity, and numbers that lie
between the whole numbers (fractions and decimals). Let's learn about them so
that we can make our _expressions_ more exciting!

## Define Reserved Word

We haven't seen any reserved words _yet_ in Ruby, but they're the words that
make Ruby do something else besides _evaluate_ an _expression_. They look like
`def` or `if` or `else` or `end`.  You can't use a reserved word as a variable
name. Ruby only has a few dozen reserved words and it will complain if you try
to assign to one with an assignment expression. We can avoid this problem by
having variables with descriptive names separated by `_`.

## Programming as Conversation: Classification to Data Types

A baby spends the first 3-5 years of their life running _assignment
expressions_ learning about "dogs," "boats," and "trains." They're gaining
variable names that they can use to "point to" the things in the world.

Eventually, after they age a bit, the children start learning more advanced
concepts like "similar" or "dissimilar" or "belonging to a group." "Sesame
Street" says it like so:

<iframe width="560" height="315" src="https://www.youtube.com/embed/rsRjQDrDnY8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

We call the classifications that data can be sorted into "data types."

## Name the Scalar Data Types in Ruby

The five _scalar_ data types are:

* `Integer`
* `Float`
* `Boolean`
* `String`
* `Symbol`

What does "_scalar_" mean? It means things that could be put on a _scale_. All
of the following are _scalar_ values.

![Image of Scales of Scalar Data](https://curriculum-content.s3.amazonaws.com/programming-univbasics/data-types/Image_89_ScalarDataTypes.png)

"Scalar" is often used to mean "atomic" or "simple." You'll get the hang of
this term as we go on.

## Identify an `Integer`

There's a number _scale_ for whole numbers, or `Integer`s (-1, 0, 1, ...).
You've created several `Integer` constants in this module.

## Identify a `Float`

There's a number _scale_ for `Float`ing point numbers
(-0.0001...0....1,000,000).  Create `Float`s the same way you create
`Integer`s: simply type them in.

## Identify Boolean Values

The mathematics of _expressions_ made up only of `true` and `false` was
established by George Boole, an English mathematician. In his honor, the
_scale_ of values between `true` and `false` are called "Boolean." To use these
in Ruby expressions, you just type in `true` or `false`

## Identify `String` Values

You create `String`s by surrounding text in `""` or `''`. We'll only use `""`
for the time being, though.  You might be OK with considering `true` and
`false` as being on a scale, and thus _scalar_; and you're probably OK with
numbers like `Float`s and `Integer`s being on a scale, and thus _scalar_; but
the following might sound strange: `String`s are also considered scalar because
computers see `String`s as collections of numbers.

## Identify `Symbol` Values

The last data type we'll discuss is a `Symbol`. It's like a `String` but it's
usually used when we intend for the `String` to act more like a label. They
look like  `:i_am_a_symbol` or `:razzmatazz`. It's a _scalar_ because of the
same logic as behind a `String`.

## Ask IRB for the Data Type of a Value

Try assigning these types of data to a new variable in IRB. For example:

```ruby
beauty = true  # Profound! Is beauty `true`?
angels_on_a_pinhead = 1345891
precise_angels_on_a_pinhead = 1345891.0141125125
```

Amazingly, Ruby will tell us what kind of type a given piece of data is if we
add `.class` to the end of a _scalar value_:

```ruby
10.class #=> Fixnum
10.0.class #=> Float
true.class #=> TrueClass
false.class #=> FalseClass
"A fellow of infinite jest".class #=> String
:byron_the_poodle.class #=> Symbol
```

Ruby says that `10` is a `Fixnum`. A `Fixnum` is a number without a decimal, an
`Integer`. We'll learn more about how `.class` works when we get a bit farther
along.  For now, it's enough to know that you can ask data about itself in Ruby
(pretty amazing).

## Conclusion

OK! So you've now discovered the "types" of data in Ruby. You should now use
IRB to try the _essential three_ expressions with these new types of data. Look
at a _constant expression_ with `String`; write an _assignment expression_ with
a variable and a `String`; lookup the content of the variable and make sure you
get your `String` back out.
