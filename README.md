#Introduction
This project provides simple extension methods for handling argument validation in a fluent form.

#Examples
Here's some examples of how it can be used...

  public void MyMethod(object param1)
  {
      param1.ThrowIfNull(nameof(param1));     
  }

  public void MyMethod(string param1)
  {
      param1.ThrowIfNullOrEmpty(nameof(param1));    
  }

It is fully fluent, returning the original object, allowing methods like this...

  public int Increment(int? param1)
      => param1.ThrowIfNull(nameof(param1)) + 1;