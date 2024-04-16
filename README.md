Sure! Here's an implementation of factorial in 10 different programming languages, including C# and Python:

1. **C#**
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Enter a number:");
        int num = Convert.ToInt32(Console.ReadLine());
        int result = 1;
        for (int i = 1; i <= num; i++)
        {
            result *= i;
        }
        Console.WriteLine($"Factorial of {num} is {result}");
    }
}
```

2. **Python**
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

num = int(input("Enter a number: "))
print(f"Factorial of {num} is {factorial(num)}")
```

3. **Java**
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter a number:");
        int num = scanner.nextInt();
        int result = 1;
        for (int i = 1; i <= num; i++) {
            result *= i;
        }
        System.out.println("Factorial of " + num + " is " + result);
    }
}
```

4. **JavaScript**
```javascript
function factorial(n) {
    if (n === 0) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}

let num = parseInt(prompt("Enter a number: "));
console.log(`Factorial of ${num} is ${factorial(num)}`);
```

5. **Ruby**
```ruby
def factorial(n)
  n == 0 ? 1 : n * factorial(n - 1)
end

print "Enter a number: "
num = gets.chomp.to_i
puts "Factorial of #{num} is #{factorial(num)}"
```

6. **C++**
```cpp
#include <iostream>
using namespace std;

int factorial(int n) {
    return (n == 0) ? 1 : n * factorial(n - 1);
}

int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    cout << "Factorial of " << num << " is " << factorial(num) << endl;
    return 0;
}
```

7. **Swift**
```swift
func factorial(_ n: Int) -> Int {
    return n == 0 ? 1 : n * factorial(n - 1)
}

print("Enter a number:")
if let num = Int(readLine()!) {
    print("Factorial of \(num) is \(factorial(num))")
}
```

8. **PHP**
```php
<?php
function factorial($n) {
    return $n == 0 ? 1 : $n * factorial($n - 1);
}

echo "Enter a number: ";
$num = intval(fgets(STDIN));
echo "Factorial of $num is " . factorial($num) . "\n";
?>
```

9. **Rust**
```rust
use std::io;

fn factorial(n: u64) -> u64 {
    match n {
        0 => 1,
        _ => n * factorial(n - 1),
    }
}

fn main() {
    println!("Enter a number:");
    let mut input = String::new();
    io::stdin().read_line(&mut input).expect("Failed to read line");
    let num: u64 = input.trim().parse().expect("Please enter a number");
    println!("Factorial of {} is {}", num, factorial(num));
}
```

10. **Haskell**
```haskell
factorial :: Integer -> Integer
factorial 0 = 1
factorial n = n * factorial (n - 1)

main :: IO ()
main = do
    putStrLn "Enter a number:"
    num <- readLn
    putStrLn $ "Factorial of " ++ show num ++ " is " ++ show (factorial num)
```

These are implementations of the factorial function in 10 different languages, including C# and Python.