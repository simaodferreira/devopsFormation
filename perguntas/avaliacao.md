# Perguntas de escolha multipla

1. Para o traefik funcionar e preciso os docker terem os ports expostos?
  sim
  nao

2. Os dockeres tem de estar a correr na mesma networks para o traefik conseguir roterar?
  sim
  nao

3. Qual das das seguinte linha é valida?
  "traefik.http.routers.whoami=PathPrefix(`/route`)"
  "traefik.http.routers.whoami.rule=PathPrefix(`/route`)"
  "traefik.http.routers.helloworld.PathPrefix=(`/route`)"
  "traefik.http.routers.helloworld.rule.PathPrefix=(`/route`)"

4. Os 2 conjuntos de linhas seguinte significam o mesmo?

  a)
  traefik.http.routers.helloworld.rule=PathPrefix(`/route`)"
  traefik.http.routers.helloworld.service=helloworld-svc

  b)
  traefik:
    http:
      routers:
        helloworld:
          rule: PathPrefix(`/route`)"
          service: helloworld-svc  
