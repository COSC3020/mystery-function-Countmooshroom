[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11730499&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

# Answer
This function takes an array as an argument.  If the array has only one item, it returns that item.  Otherwise, it makes a recursive call to run the function again with the same array except the first item is taken off.  Then, if the return value from the recursion is greater than the first item in the array, it returns the value from the recursion.  Otherwise, it returns the first item in the array.

Ultimately, the function just finds the highest value in an array.
