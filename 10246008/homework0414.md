1.請完成以下實作練習：

```
class Animal
  def sleep
    puts "ZZZZZZ"
  end
  def eat
    puts "Yammy!"
  end
end

class Cat < Animal; end
class Dog < Animal; end

kitty = Cat.new
kitty.sleep     # => "ZZZZZZ"

lucky = Dog.new
lucky.eat       # => "Yammy!"
```

2.請完成以下實作練習：

```
class Cat
  attr_accessor:age
  def initialize(age)
    @age=age
  end
end

kitty = Cat.new(10)
puts kitty.age       # => 10
kitty.age = 18
puts kitty.age       # => 18
```

3.請完成以下實作練習：

```
module Flyable
  def fly
    puts "I can fly!!"
  end
end

class Cat
include Flyable
end

kitty = Cat.new
kitty.fly         # => "I can fly!!"
```

4.請寫一段 Ruby 程式，讓 `puts "hello world".count_character` 可以在畫面上印出 `10`
```
class String
  def count_character
    self.length - self.count(" ")
  end
end
puts "hello world".count_character
```

5.請簡述或使用程式碼說明在 Ruby 中 `public`、`protected` 以及 `private` 有何不同?
```
public大家都可以使用
private前面不能有小數點(接收者)
protected可以有小數點(接收者)
```
