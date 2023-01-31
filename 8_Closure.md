**Python Closures**
is a nested function that allows us to access variables of the outer function even after the outer function is closed.


def greet():
# variable defined outside the inner function
    name = "John"
    
# return a nested anonymous function
    return lambda: "Hi " + name

# call the outer function
message = greet()

# call the inner function
print(message())

# Output: Hi John