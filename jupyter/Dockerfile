FROM jupyter/datascience-notebook

RUN python --version

RUN conda install --quiet --yes -c \
    conda-forge osmnx dask

RUN pip install -U geopandas \
                   geopy \
                   rtree \
                   folium \
                   numpy \
                   shapely \
                   fiona \
                   six \
                   pyproj \
                   elasticsearch \
                   geojson \
                   plotly \
                   tqdm \
                   mapboxgl \
                   cufflinks \
                   geohash2 \
                   tables \
                   mixpanel \
                   SQLAlchemy \
                   GeoAlchemy2

ADD fonts /usr/share/fonts/truetype/

RUN fc-cache
RUN fc-list

VOLUME /notebooks
WORKDIR /notebooks
