## cert problems

save yourself the pain of SSL error and PKIX path building exceptions by adding the following flag:

`-Djavax.net.ssl.trustStoreType=WINDOWS-ROOT`

this automatically trusts the windows cert store, which should ease things in enterprise locations
