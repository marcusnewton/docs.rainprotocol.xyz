Factory for creating and deploying `VerifyTier` contracts.


## Variables
### `address` `implementation`




## Functions
### `constructor()` (public)

Build the reference implementation to clone for each child.



### `_createChild(bytes data_) → address` (internal)

Implements `IFactory`.

`_createChild` hook must be overridden to actually create child
contract.

Implementers may want to overload this function with a typed equivalent
to expose domain specific structs etc. to the compiled ABI consumed by
tooling and other scripts. To minimise gas costs for deployment it is
expected that the tooling will consume the typed ABI, then encode the
arguments and pass them to this function directly.





### `createChildTyped(address verify_) → contract VerifyTier` (external)

Typed wrapper for `createChild` with `Verify`.
Use original `Factory` `createChild` function signature if function
parameters are already encoded.





