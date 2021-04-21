This branch includes a cook-encryption.properties file that has
the `cook.special` property set to an encrypted value. This is
different from the same file in the `master` branch because it
seems that the private key that matches the public key used to
value in that file may have been lost and therefore, difficult
to use when demonstrating or testing encrypted properties.

So as not to lose the private key used to sign this branch's
value, both the public and private keys in play are in LastPass
in the entry named "Cook Config Key Pair" under "Shared-Spring
Cloud Services".

At some point, as a point of cleanup, this branch could be
merged into `master` and the encrypted value changed to be one
that was encrypted with the known public key. For now, however,
to avoid breaking anything unintentionally, the old value will
remain in the `master` branch.
