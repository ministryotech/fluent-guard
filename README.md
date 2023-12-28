This project provides simple extension methods for handling argument validation in a fluent form.

# Examples
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
        
# Available Methods
The following fluent error checks are available along with the exceptions they can generate (depending on the value)...
- **ThrowIfNull** - ArgumentNullException
- **ThrowIfNullOrEmpty** - ArgumentNullException / ArgumentException
- **ThrowIf** - ArgumentException
- **ThrowOutOfRangeIf** - ArgumentOutOfRangeException

## The Ministry of Technology Open Source Products
Welcome to The Ministry of Technology open source products. All open source Ministry of Technology products are distributed under the MIT License for maximum re-usability.
Our other open source repositories can be found here...

* [https://github.com/ministryotech](https://github.com/ministryotech)
* [https://github.com/tiefling](https://github.com/tiefling)

### Where can I get it?
You can download the package for this project from any of the following package managers...

- **NUGET** - [https://www.nuget.org/packages/Ministry.FluentGuard](https://www.nuget.org/packages/Ministry.FluentGuard)

### Contribution guidelines
If you would like to contribute to the project, please contact me.

### Who do I talk to?
* Keith Jackson - temporal-net@live.co.uk