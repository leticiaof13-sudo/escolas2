# Mapa de Escolas

Mapa interativo com **351 escolas** (municipais, estaduais, particulares, CEMEI, CEI, FUNEC etc.), com busca por nome e filtro por tipo. As coordenadas originais (SIRGAS 2000 / UTM 23S) foram convertidas para latitude/longitude.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (público), por exemplo `mapa-escolas`.
2. Faça upload destes 2 arquivos para a raiz do repositório:
   - `index.html`
   - `schools_data.js`
3. No repositório, vá em **Settings → Pages**.
4. Em "Source", selecione a branch `main` e a pasta `/ (root)`. Clique em **Save**.
5. Aguarde 1–2 minutos. O mapa ficará disponível em:
   `https://SEU-USUARIO.github.io/mapa-escolas/`

## Estrutura

```
index.html        # página do mapa (Leaflet + OpenStreetMap)
schools_data.js    # dados das escolas (nome, tipo, lat, lon)
```

## Editar os dados

Os dados estão em `schools_data.js` como uma lista de objetos:

```js
const SCHOOLS = [
  {"name":"Coronel Antonio Augusto Diniz Costa","tipo":"Escola Municipal","lat":-19.932024,"lon":-44.086297},
  ...
];
```
