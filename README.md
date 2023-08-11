# oem-database-config-deploy
[https://andrew-b-shaw.github.io/oem-database-config-deploy/](https://andrew-b-shaw.github.io/oem-database-config-deploy/)

## Fields
- Title: The title of the layer.
- URL: The ArcGIS feature service URL for the layer. ArcGIS feature services may contain multiple layers, which are indicated by the numerical suffix at the end of the URL. For example, https://services1.arcgis.com/UWYHeuuJISiGmgXx/arcgis/rest/services/Neighborhood/FeatureServer/0 is the first (0-indexed) layer in the Neighborhood Feature Server. If the layer is not specified, ArcGIS will automatically use the first layer in the feature server. To reduce network request time, always specify the layer index, even if the feature service only contains 1 layer. For example, use https://services1.arcgis.com/UWYHeuuJISiGmgXx/arcgis/rest/services/Neighborhood/FeatureServer/0 instead of https://services1.arcgis.com/UWYHeuuJISiGmgXx/arcgis/rest/services/Neighborhood/FeatureServer.
- Scope: The geographical scope of the layer. Common scopes include Baltimore, MD (Maryland), and US.
- Source: The author or source of the layer.
- Description: A description of the layer metadata.
- Category ID: The ID of the associated category from the Categories table.
- Renderer (Optional): Used to specify a custom [Renderer](https://developers.arcgis.com/javascript/latest/api-reference/esri-renderers-Renderer.html) for the layer in JSON format. If not specified, the default renderer from the layer URL will be used.
