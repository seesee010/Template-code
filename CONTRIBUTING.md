# Contributing to my Project
Thanks for your interest in contributing! Here's how you can help:

## How to Contribute

1. Fork the repository
2. Create a branch following this pattern:
    - `feature/<name>` for new features
    - `fix/<name>` for fixes
    - `chores/<name>` for administrative changes: (README (/ docs), config files, by cleaning code)
    - `refactor/<name>` if you change the structure
    - `hotfix/<name>` if you want to change code, which is already live and need a very fast update (/ critical updates)

    Only use following chars:
    - a to z
    - A to Z
    - 0 to 9
    - @, #, ö, ü, ä, ß, $, € (very rare but allowed)
    - -, +

3. Make your changes and commit using the commit template.
4. Push your branch to your fork.
5. Open a Pull Request.

## Code of Conduct
Please follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Reporting Bugs

- Use the Issues tab.
- Everying is an issue
- Provide a clear describtion, and use the issue template!

## Style Guidelines

### General

#### Variable
- Keep the name short and focused
- do NOT use nonsense names!

### In every language:
(code is mostly in C and aplies mostly onto C)

#### Func names
- Keep the name short and focused
- do NOT use nonsense names!

If you create a func, you MUST always use a context!
Like this here: `matrix_init();` here you can instant see that "matrix_" is a prefix/namespace,
and it clearance that the func is from / for "matrix"... another example:
`http_requestSend();`, which will create a request...

> Here you know from the lines of code that the requestSend() func is for http... 
> if there whould stand: `requestSend();` you wouldn't know for what that is!

This does also mean that this princible will remove a lot of comments.

#### Consistant spaces & tabs
You need to add **1** space before and after an `=`,
that whould look like:

```c
int a = 1;
```

An if statement must look like:

```c
if (condition) {
    // new code here

}
else {
    // new code here
}
```

> Every time you create an if statement you will need to go ones deeper.

There MUST be ==**ONE**== space between your code inside your if and the ending of and if / else / func etc!

Like:

```c
if (condition) {
    // here is my new code
    a = 10;

}
```

> If there is an if do ==NEVER== use this version: `if (condition) a = 10;`

here is how code should look like (==tabs==) (==**1 tab = 4 spaces**==):
```c
void main(void) {
    // 1 tab
    if (condition) {
        // 2 tabs
    }
}
```

> Do NOT nest code (like over ~4).

> Do ALWAYS add 1 space after an comment char/s and your comment

```c
// this is correct!

//no never use this!
```

> do never use an space after all code! (/ at the end of a file)

```c

void main(void) {
    // your code

}
// the extra line is forbidden!

```

Always write new code after blocks (if / switches / func / else / ...)
with 1 space before!

```c
if (condition) {
    // your code here
}

// there is one space between this comment and the if statement!
```

> There is NO space between the function and the brackets!

```c
void main(void) {
    // your code here

}
```

and there is no space in between these brackets!

## Review Process

- Your PR will be reviewed by a maintainer.
- Adress review comments proptly.
- Once approved, your changes will be merged

> Use the PR template!

## Credits
Done by @seesee010