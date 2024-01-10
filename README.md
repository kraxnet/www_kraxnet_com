# kraxnet.com website

Jekyll based website hosted as github pages.

## security.txt


This website includes a security.txt file, which requires regular review, and its expiration should be extended at least once a year. 

After each modification, the file needs to be re-signed.  Please remove the header and signature sections:

```
-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA256

-----BEGIN PGP SIGNATURE-----

<signature to be removed>
-----END PGP SIGNATURE-----
```

Then sign and rename new plaintext file:

``` shell
GNUPGHOME=~/.gnupg/trezor gpg --clearsign .well-known/security.txt
mv .well-known/security.txt.asc .well-known/security.txt
```
