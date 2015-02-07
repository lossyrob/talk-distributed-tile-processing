# Distributed tile processing w/ GeoTrellis and spark.

# Describe the challenges
 - Describe the climate data set
 - Describe the OTM data sets

# Describe the technologies
 - GeoTrellis: a scala library for doing anything geospatial
 - Spark: Cluster computing

# How we store tiles
 - Distributed Data Stores: Accumulo and HDFS

# Ingesting tiles
 - Describe the process. Show what it looks like.
 - Example: ingesting the housing vacancy raster.
   - Tile using GDAL gdal_retile.py
   - Upload to S3 in chunks of GeoTIFFS
   - Reproject the tiles
   - Combine the tiles per key

# Serving tiles
  - Describe challenge of filtering spatiall

# Temporal component
  - Time series rasters produce an additional challenge
  - Band rasters as well.


# FOSSDEM presentation:

Python tiling takes 3 minutes to complete.

Talk about why we need to use accumulo while ingest is taking place.

Have the viewer running. Show that it wasn't there, then show that it is there.
View the data in the viewer.

Open up a shell, start doing calculations. Save off data. Show in the viewer.


Brain dump for another talk:
                                    Minimizing Shuffling.
                                    Maximizing Distribution.
                                    Minimize Query cost.

                                    How z curve fits those roles. Some examples. Some graphics.
                                    What it takes to index tiles with a z curve.
                                    How GeoTrellis makes this pretty.


