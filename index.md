# Class Vs. Instance

#### [HackerRank](www.hackerrank.com)

## Problem

Defined by [HackerRank](www.hackerrank.com).

> Write a Person class with an instance variable, age, and a constructor that takes an integer, initialAge, as a parameter.
The constructor must assign initialAge to age after confirming the argument passed as initialAge is not negative;
if a negative argument is passed as initialAge, the constructor should set  to  and print Age is not valid,
setting age to 0.. In addition, you must write the following instance methods:

> 1. yearPasses() should increase the  instance variable by 1.
> 1. amIOld() should perform the following conditional actions:
  > * If < 13, print You are young..
  > * If ≥ 13 and < 18, print You are a teenager..
  > * Otherwise, print You are old..
  
## Template

```
class Person:
    def __init__(self,initialAge):
    def amIOld(self):
    def yearPasses(self):


t = int(input())
```
  
## Solve

#### Define A Problem

> "...if a negative argument is passed as initialAge, the constructor should set  to  and print Age is not valid,
> setting age to 0."

Pretty straight forward.

#### Thought Process

```
# if initialAge < 0 print age is not valid, setting age to 0
# else set self.initialAge to initialAge
```

#### Code

```
...
def __init__(self,initialAge):
  if initialAge < 0:
    print("Age is not valid, setting age to 0.")
    self.initialAge = 0
  else:
    self.initialAge = initialAge
...
```

#### Define A Problem

> "yearPasses() should increase the  instance variable by 1."

#### Thought Process

```
# age = age + 1
```

#### Code

```
...
def yearPasses(self):
  self.initialAge = self.initialAge + 1
...
```

#### Define A Problem

> amIOld() should perform the following conditional actions:
  > * If < 13, print You are young..
  > * If ≥ 13 and < 18, print You are a teenager..
  > * Otherwise, print You are old..
  
#### Thought Process

```
# if age < 13 print you are young
# else if age ≥ 13 and < 18 print you are a teenage
# else print you are old
```

#### Code

```
...
def amIOld(self):
  if self.initialAge < 13:
    print("You are young.")
  elif self.initialAge >= 13 and self.initialAge < 18:
    print("You are a teenager.")
  else:
    print("You are old.")
...
```

## Final Code

```
class Person:
  def __init__(self,initialAge):
    if initialAge < 0:
      print("Age is not valid, setting age to 0.")
      self.initialAge = 0
    else:
      self.initialAge = initialAge
  def amIOld(self):
    if self.initialAge < 13:
      print("You are young.")
    elif self.initialAge >= 13 and self.initialAge < 18:
      print("You are a teenager.")
    else:
      print("You are old.")
  def yearPasses(self):
  se  lf.initialAge = self.initialAge + 1

t = int(input())
```

## Conclusion
This was probably one of the easier ones to tackle but does not mean it is not good practice. The only easy day was yesterday.
