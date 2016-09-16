## Ruby is dynamically typed

What happens when we execute this program without arguments?

```
if ARGV.empty?
  x = 1
else
  x = "hi"
end

puts x + 2
```

Note:
It works! Ruby executes the "then" branch, assigning the value 1, which is of class `Fixnum`, to `a`. It never analyses the "else" branch. It then analyses the `a + 2`, and because `a` is `Fixnum` at that moment, it works.

In a dynamically typed language, a variable's type can change during execution, and methods are looked up relative to that type at each moment.