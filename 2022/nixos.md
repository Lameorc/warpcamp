# Nix(OS)
- Prakticky jsou to 3 veci
    - Konfiguracni jazyk
    - OS
    - Balickovaci system

- Deklarativni prostredi
  - i balicky
- "Balicek" je
- "Vse" je soucast nixpkgs monorepa na githubu
- Nove jeste flakes (deklarace mimo hlavni monorepo)


# Ukazka na k6
```sh
# clone repo
git clone https://github.com/grafana/k6-template-typescript.git grafana/k6-template-typescript

# cd in
cd grafana/k6-template-typescript

# ad-hoc dev-env - balicky podle readme
nix-shell -p yarn nodejs k6

# inside nix-shell now
yarn install
NODE_OPTIONS=--openssl-legacy-provider yarn webpack
```


# Reference
- https://search.nixos.org/packages
- https://mat.services/posts/static-site-with-nix-and-caddy/
- https://xeiaso.net/blog/nix-flakes-1-2022-02-21
- https://xeiaso.net/blog/nix-flakes-2-2022-02-27
