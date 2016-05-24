xxHashSharp
===========

A pure C# implementation of [xxhash](http://code.google.com/p/xxhash/)


## Installation

1. From Nuget

 * Download from [Nuget](https://www.nuget.org/packages/xxHashSharp/)
 * Also, run the following command in the Package Manager Console.

   ```
   PM > Install-Package xxHashSharp
   ```

2. From Source
 * You can just clone this repo.


## Example

```csharp
byte[] input = Encoding.UTF8.GetBytes("hello world");

xxHash hash = new xxHash();
hash.Init();
hash.Update(input, input.Count());
...
Console.WriteLine("{0:X}", hash.Digest());
```	

or

```csharp

byte[] input = Encoding.UTF8.GetBytes("hello world");
Console.WriteLine("{0:X}", xxHash.CalculateHash(input));
```

## License

BSD 2-clause license.
