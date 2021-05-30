# Copying Objects
## Copy Constructor

Example of a Map template function for mapping property contents of one object (class) to another:
https://stackoverflow.com/questions/14613919/copying-the-contents-of-a-base-class-from-a-derived-class

Example with explicit base class property copying:
https://stackoverflow.com/questions/4823766/derived-and-base-class-can-i-set-the-base-explicitly/19010127#19010127

## Shallow Copy

## Deep Copy

## MemberwiseClone Method (MS)
However this solutions only works the other way round - get a copy from an object, it's not going to work with a copy constructor.
https://docs.microsoft.com/en-us/dotnet/api/system.object.memberwiseclone?redirectedfrom=MSDN&view=net-5.0#System_Object_MemberwiseClone

## ICloneable Interface
Different approach to MemberwiseClone, but similar result and not working in a constructor.
Major drawback is that Microsoft never defined whether Clone should be a shallow or deep copy. 
Therefore the Interface is ambiguous and *must not be used*.
An alternative would be to define IDeepCloneable or IShallowCloneable.
https://docs.microsoft.com/en-us/dotnet/api/system.icloneable?redirectedfrom=MSDN&view=net-5.0

### great arguments about copy constructor vs. icloneable
In short: both are needed and ok. Deep vs shallow should not be of concern for the caller - the 'contract' is to provide a copy
that can be altered independently from the original - how deep the copy needs to be is to be determined by the providing developer.
https://stackoverflow.com/questions/3345389/copy-constructor-versus-clone
