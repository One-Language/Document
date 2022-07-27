# Syntax

One’s syntax is designed to be familiar to people coming from C-like languages while being a bit simpler and more streamlined.

Scripts are stored in plain text files with a `.one` file extension. One does not compile ahead of time: programs are run directly from source, from top to bottom like a typical scripting language. Internally, programs are compiled to bytecode for efficiency, but that’s an implementation detail.

## Comments

Line comments start with // and end at the end of the line:

```
// This is a comment.
```

<!-- prettier-ignore-start -->
Block comments start with /* and end with */. They can span multiple lines: <!-- markdownlint-disable MD037 -->
<!-- prettier-ignore-end -->

```
/* This
   is
   a
   multi-line
   comment. */
```

Unlike C, block comments can nest in One:

```
/* This is /* a nested */ comment. */
```

This is handy because it lets you easily comment out an entire block of code, even if the code already contains block comments.

## Reserved words

One way to get a quick feel for a language’s style is to see what words it reserves. Here’s what One has:

```
as break class construct continue else false for foreign if import
in is null return static super this true var while
```

## Identifiers

Naming rules are similar to other programming languages. Identifiers start with a letter or underscore and may contain letters, digits, and underscores. Case is sensitive.

```
hi
camelCase
PascalCase
_under_score
abc123
ALL_CAPS
```

Identifiers that start with underscore (`_`) are special in One. They are used to indicate fields in classes.

## Newlines

Newlines (\n) are meaningful in One. They are used to separate statements:

```
// Two statements:
System.print("hi") // Newline.
System.print("bye")
```

Sometimes, though, a statement doesn’t fit on a single line and jamming a newline in the middle would trip it up. To handle that, One has a very simple rule: It ignores a newline following any token that can’t end a statement.

```
System.print( // Newline here is ignored.
    "hi")
```

In practice, this means you can put each statement on its own line and wrap them across lines as needed without too much trouble.
