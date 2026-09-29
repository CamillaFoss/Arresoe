# Arresø
Min legeplads til at bringe min sø-modelleringsviden up-to-date
![Arresø google map d. 27. sept. 2026](Arresoe_google_20260927.png)

Googles bud på en bounding_box er ikke god nok 
- Brug datafordeleren til at hente sø-geometri

DS_Stednavn (skrivemaade, navngivetSted_objectid)
DS_Soe (objectid, geometri)
ETRS89 / UTM zone 32N (EPSG:25832)

GEODKV_Soe

https://geodanmark.nu/Spec6/HTML5/DK/StartHer.htm
- Brug geojson-formatet i projektionen WGS 84 (EPSG:4326) og få kortvisning i github 

```
library(sf)

# 1. Indlæs din danske EPSG:25832 GeoJSON-fil
# (R vil typisk automatisk genkende projektionen fra filen)
kort_data <- st_read("datafordeler_geometri.geojson")

# 2. Sikkerheds-tjek: Hvis filen mangler CRS-information, definerer vi den som 25832
if (is.na(st_crs(kort_data))) {
  kort_data <- st_set_crs(kort_data, 25832)
}

# 3. Transformer koordinaterne til WGS 84 (EPSG:4326) til GitHub
kort_data_github <- st_transform(kort_data, crs = 4326)

# 4. Gem den nye fil, klar til upload
st_write(kort_data_github, "github_klar_geometri.geojson", driver = "GeoJSON", delete_dsn = TRUE)

```

- Bestem kvadrater i DKN 

![Arresø med DKN 1km](Arresoe_med_1km_kvadrater.png)

Inspiration 
https://sgavmst.dk/media/kxspz2ao/dokumentation-for-digitalt-skovkort.pdf