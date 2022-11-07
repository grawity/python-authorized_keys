Parser for `authorized_keys` files

Unlike a basic `split(" ")`, this module aims to handle arbitrary OpenSSH
option prefixes (including quoted values that might confuse the hell out of
other parsers) **and** arbitrary key type prefixes (including those which do
not start with `ssh-` or `ecdsa-`).

Originally written as part of the `ssh-publickeyd` RFC4819 implementation.
