# plutus_projects

I found setting up plutus playground incredibly unclear and all the documentation surrounding misleading and or out of date.

1) git clone plutus repository
2) install nixOS from shell script method
3) nix-shell in plutus
4) git clone plutus-apps repository (actual home of plutus playground)
5) nix-shell in plutus-apps
6) launch frontend via plutus-playground-frontend run `npm run start`
7) configure web-ghc (edit code or otherwise assign port to web-ghc)
8) launch backend AND web-ghc
9) $(nix-build -A plutus-playground.server)/bin/plutus-playground-server webserver
10) $(nix-build -A web-ghc)/bin/web-ghc-server webserver
11) enjoy
