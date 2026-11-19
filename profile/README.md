<div align="center">

# Siradel Open Source

**Open-source building blocks for 3D geospatial applications and digital twins.**

[Website](https://sce.oss.siradel.com) ·
[Horizon 3D engine](https://github.com/siradel-oss/horizon) ·
[Live demos](https://sce.oss.siradel.com/demos/) ·
[YouTube](https://www.youtube.com/@siradel2026) ·
[Contact](mailto:opensource@siradel.com)

</div>

[Siradel](https://www.siradel.com) is a French company building 3D geospatial
software for cities, networks and territories. This organization publishes the
open-source components of **SCE**, its geospatial ecosystem: process, serve and
visualize geospatial data in 2D and 3D, on the web and natively, from maps to
digital twins.

## Horizon, the 3D engine

<a href="https://github.com/siradel-oss/horizon"><img src="https://raw.githubusercontent.com/siradel-oss/horizon/HEAD/public/terrain.webp" alt="Terrain rendered by the Horizon 3D engine" width="100%"></a>

[**Horizon**](https://github.com/siradel-oss/horizon) is a real-time 3D engine
for map data on a globe. It runs in the browser (WebAssembly, WebGL 2,
TypeScript) and natively on Windows and Linux (C++, OpenGL), through one
language-independent API.

- **Terrain and imagery** streamed worldwide down to centimetre resolution:
  WMS, WMTS, TMS, PMTiles, TileJSON, ArcGIS…
- **Vector data** in 3D: GeoJSON, MVT, PMTiles, extrusions, instanced models,
  heatmaps, scripted styling, Mapbox style import.
- **3D models**: glTF, 3D Tiles and point clouds, at any scale.
- **Analysis and interaction**: picking, gizmos, viewshed, clipping, in-view
  editing, multi-view.

```sh
npm install @siradel-oss/horizon-core @siradel-oss/horizon-api
```

[Getting started](https://horizon.oss.siradel.com/doc/getting_started.html) ·
[Documentation](https://horizon.oss.siradel.com/) ·
[Releases](https://github.com/siradel-oss/horizon/releases) ·
[Discussions](https://github.com/siradel-oss/horizon/discussions)

If Horizon is useful to you, a ⭐ on the
[repository](https://github.com/siradel-oss/horizon) helps others find it.

## Demos

Open-source web applications built on Horizon with open data. Each one has a
live version and its full source code.

<table>
  <tr>
    <td width="33%" valign="top">
      <a href="https://oss.siradel.com/horizon-demo-reunion-island/"><img src="https://raw.githubusercontent.com/siradel-oss/horizon-demo-reunion-island/HEAD/.github/screenshot.webp" alt="Hiking trail in the Cilaos cirque on a 3D model of Reunion Island"></a>
      <br><b>Reunion Island Explorer</b>
      <br>Hiking trails with elevation profiles, drone flyovers and LiDAR trees.
      <br><a href="https://oss.siradel.com/horizon-demo-reunion-island/">Live demo</a> · <a href="https://github.com/siradel-oss/horizon-demo-reunion-island">Code</a>
    </td>
    <td width="33%" valign="top">
      <a href="https://oss.siradel.com/horizon-demo-ign-geoplateforme/"><img src="https://raw.githubusercontent.com/siradel-oss/horizon-demo-ign-geoplateforme/HEAD/.github/screenshot.webp" alt="IGN Géoplateforme relief on a 3D globe"></a>
      <br><b>IGN Explorer</b>
      <br>The IGN Géoplateforme catalogue on a 3D globe: WMTS, WMS, vector tiles, elevation.
      <br><a href="https://oss.siradel.com/horizon-demo-ign-geoplateforme/">Live demo</a> · <a href="https://github.com/siradel-oss/horizon-demo-ign-geoplateforme">Code</a>
    </td>
    <td width="33%" valign="top">
      <a href="https://oss.siradel.com/horizon-demo-coastline-erosion/"><img src="https://raw.githubusercontent.com/siradel-oss/horizon-demo-coastline-erosion/HEAD/.github/screenshot.webp" alt="Projected 2100 coastline retreat shown in 3D"></a>
      <br><b>Shoreline Explorer</b>
      <br>Coastal erosion in France: historical coastlines and 2050/2100 projections.
      <br><a href="https://oss.siradel.com/horizon-demo-coastline-erosion/">Live demo</a> · <a href="https://github.com/siradel-oss/horizon-demo-coastline-erosion">Code</a>
    </td>
  </tr>
</table>

All demos: [sce.oss.siradel.com/demos](https://sce.oss.siradel.com/demos/)

## Websites

| Site | What you will find |
| --- | --- |
| [sce.oss.siradel.com](https://sce.oss.siradel.com) | The SCE ecosystem, its building blocks and the demo gallery |
| [horizon.oss.siradel.com](https://horizon.oss.siradel.com) | Horizon documentation, guides and API reference |
| [siradel.com](https://www.siradel.com) | Siradel, products and enterprise offers |

## Other repositories

- [bazel-registry](https://github.com/siradel-oss/bazel-registry): Siradel's Bazel modules
- [glslang-prebuilt](https://github.com/siradel-oss/glslang-prebuilt) and
  [clang-format-prebuilt](https://github.com/siradel-oss/clang-format-prebuilt):
  prebuilt tools as Bazel modules
- [sce-website](https://github.com/siradel-oss/sce-website) and
  [horizon-website](https://github.com/siradel-oss/horizon-website): the sources of our websites

## Get involved

- Questions and ideas: [Horizon discussions](https://github.com/siradel-oss/horizon/discussions)
- Bugs and feature requests: open an issue in the relevant repository
- First contribution: [good first issues](https://github.com/search?q=org%3Asiradel-oss+is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22&type=issues)
- Before contributing: [contributor guide](https://github.com/siradel-oss/.github/blob/main/CONTRIBUTING.md)
  and [code of conduct](https://github.com/siradel-oss/.github/blob/main/CODE_OF_CONDUCT.md)

Enterprise support and partnerships: [opensource@siradel.com](mailto:opensource@siradel.com)

<sub>Maintainers: [creating an open-source project](https://github.com/siradel-oss/.github/blob/main/opensource-guide.md) ·
[maintenance guidelines](https://github.com/siradel-oss/.github/blob/main/maintenance-guidelines.md)</sub>
