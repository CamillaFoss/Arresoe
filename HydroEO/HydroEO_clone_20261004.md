´´´
git clone https://github.com/DHI/HydroEO
mkdir HydroEO
cd HydroEO

Cloning into 'HydroEO'...
remote: Enumerating objects: 1687, done.
remote: Counting objects: 100% (260/260), done.
remote: Compressing objects: 100% (127/127), done.
remote: Total 1687 (delta 162), reused 145 (delta 133), pack-reused 1427 (from 2)
Receiving objects: 100% (1687/1687), 57.00 MiB | 31.09 MiB/s, done.
Resolving deltas: 100% (937/937), done.

git ls-files

.github/workflows/ci.yml
.gitignore
.vscode/settings.json
CITATION.cff
CLAUDE.md
HydroEO/__init__.py
HydroEO/cli/__init__.py
HydroEO/constants.py
HydroEO/downloaders/creodias.py
HydroEO/downloaders/dem.py
HydroEO/downloaders/hydroweb.py
HydroEO/flows/__init__.py
HydroEO/flows/_clean_engine.py
HydroEO/flows/_constants.py
HydroEO/flows/_merge_engine.py
HydroEO/flows/_reservoir_download.py
HydroEO/flows/_reservoir_init.py
HydroEO/flows/_reservoir_pipeline.py
HydroEO/flows/_river_common.py
HydroEO/flows/_river_download.py
HydroEO/flows/_river_init.py
HydroEO/flows/_river_pipeline.py
HydroEO/flows/_run_config.py
HydroEO/flows/_sentinel_shared.py
HydroEO/flows/_summaries.py
HydroEO/logging_config.py
HydroEO/plotting.py
HydroEO/project.py
HydroEO/satellites/icesat2/__init__.py
HydroEO/satellites/icesat2/download.py
HydroEO/satellites/icesat2/preprocess.py
HydroEO/satellites/sentinel/__init__.py
HydroEO/satellites/sentinel/download.py
HydroEO/satellites/sentinel/preprocess.py
HydroEO/satellites/swot/__init__.py
HydroEO/satellites/swot/_download.py
HydroEO/satellites/swot/pixc.py
HydroEO/satellites/swot/preprocess.py
HydroEO/satellites/swot/raster.py
HydroEO/satellites/swot/river_profile.py
HydroEO/utils/filters/basic_filters.py
HydroEO/utils/filters/kalman.py
HydroEO/utils/filters/river_profile_filters.py
HydroEO/utils/general.py
HydroEO/utils/geometry.py
HydroEO/utils/timeseries.py
HydroEO/validation.py
HydroEO/waterbody.py
LICENSE
Makefile
README.md
configs/example_data/example_res.cpg
configs/example_data/example_res.dbf
configs/example_data/example_res.prj
configs/example_data/example_res.qmd
configs/example_data/example_res.shp
configs/example_data/example_res.shx
configs/reservoirs.md
configs/reservoirs.yaml
configs/river_profile.md
configs/river_profile.yaml
configs/rivers.md
configs/rivers.yaml
configs/swot_pixc.md
configs/swot_pixc.yaml
configs/swot_raster.md
configs/swot_raster.yaml
images/HydroEO.png
images/ICESat2BeamPattern.png
images/S3_instruments.png
images/S3_swaths.png
images/Sentinel-3.jpg
images/Sentinel-6_tracks.jpg
images/icesat2-hqprint.jpg
images/sentinel-6-instruments-payload.jpg
mkdocs.yml
pyproject.toml
tests/README.md
tests/__init__.py
***tests/conftest.py***
tests/data/README.md
tests/data/aoi.e2e.gpkg
tests/data/baselines/nuozhadu/all_cleaned_timeseries.csv
tests/data/baselines/nuozhadu/cleaned_observations/icesat2.csv
tests/data/baselines/nuozhadu/cleaned_observations/sentinel3.csv
tests/data/baselines/nuozhadu/cleaned_observations/sentinel6.csv
tests/data/baselines/nuozhadu/cleaned_observations/swot.csv
tests/data/baselines/nuozhadu/merged_progress/daily_mad_error.csv
tests/data/baselines/nuozhadu/merged_progress/kalman.csv
tests/data/baselines/nuozhadu/merged_progress/svr_linear.csv
tests/data/baselines/nuozhadu/merged_progress/svr_radial.csv
tests/data/baselines/nuozhadu/merged_timeseries.csv
tests/data/config.e2e.pixc.yaml
tests/data/config.e2e.raster.yaml
tests/data/config.e2e.rivers.yaml
***tests/data/config.e2e.yaml***
tests/test_api_contracts.py
tests/test_basic.py
tests/test_e2e_run_pipeline.py
tests/test_integration.py
tests/unit/test_cli.py
tests/unit/test_creodias_client.py
tests/unit/test_dem.py
tests/unit/test_flows.py
tests/unit/test_hydroweb.py
tests/unit/test_icesat2_fields.py
tests/unit/test_no_runtime_prints.py
tests/unit/test_project_config.py
tests/unit/test_river_profile.py
tests/unit/test_river_profile_filters.py
***tests/unit/test_sentinel_downloaders.py***
tests/unit/test_swot_downloaders.py
tests/unit/test_swot_pixc.py
tests/unit/test_swot_raster.py
tests/unit/test_timeseries.py
´´´