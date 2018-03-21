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


## The Ministry of Technology Open Source Products
Welcome to The Ministry of Technology open source products. All open source Ministry of Technology products are distributed under the MIT License for maximum re-usability. Details on more of our products and services can be found on our website at http://www.ministryotech.co.uk

Our other open source repositories can be found here...

* [https://bitbucket.org/ministryotech](https://bitbucket.org/ministryotech)
* [https://github.com/ministryotech](https://github.com/ministryotech)
* [https://github.com/tiefling](https://github.com/tiefling)

Newer content prefers Github. Bitbucket is no longer actively used.

### Where can I get it?
You can download the package for this project from any of the following package managers...

- **NUGET** - [https://www.nuget.org/packages/Ministry.FluentGuard](https://www.nuget.org/packages/Ministry.FluentGuard)

### Contribution guidelines
If you would like to contribute to the project, please contact me.

### Who do I talk to?
* Keith Jackson - keith@ministryotech.co.uk# Introduction
