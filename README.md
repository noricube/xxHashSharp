xxHashSharp
===========

A pure C# implementation of [xxhash](http://code.google.com/p/xxhash/)

Example
----------

	byte[] input = Encoding.UTF8.GetBytes("hello world");
	
	xxHash hash = new xxHash();
	hash.Update(input, input.Count());
	Console.WriteLine("{0:X}", hash.Digest());
	
or

	byte[] input = Encoding.UTF8.GetBytes("hello world");
	Console.WriteLine("{0:X}", xxHash.CalculateHash(input));

License
----------

BSD 2-clause license.