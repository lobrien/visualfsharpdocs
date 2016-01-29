# Seq.sortBy<'T,'Key> Function (F#)

Applies a key-generating function to each element of a sequence and yields a sequence ordered by keys. The keys are compared using generic comparison as implemented by [Operators.compare](http://msdn.microsoft.com/en-us/library/295e1320-0955-4c3d-ac31-288fa80a658c).

**Namespace/Module Path**: Microsoft.FSharp.Collections.Seq

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## CAPS_SYNTAX_MD

```
// Signature:
Seq.sortBy : ('T -> 'Key) -> seq<'T> -> seq<'T> (requires comparison)

// Usage:
Seq.sortBy projection source
```

#### CAPS_PARAMETERS_MD
*projection*
Type: **'T -&gt; 'Key**


A function to transform items of the input sequence into comparable keys.


*source*
Type: [seq](http://msdn.microsoft.com/en-us/library/2f0c87c6-8a0d-4d33-92a6-10d1d037ce75)**&lt;'T&gt;**


The input sequence.



**exceptions tag is not supported!!!!**
**The result sequence.**
## CAPS_REMARKS_MD
This function returns a sequence that digests the whole initial sequence as soon as that sequence is iterated. Therefore, this function should not be used with large or infinite sequences. The function makes no assumption on the ordering of the original sequence. This is a stable sort, that is, the original order of equal elements is preserved.

This function is named **SortBy** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.Seq Module &#40;F&#35;&#41;](Collections.Seq+Module+%28F%23%29.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+%28F%23%29.md)
