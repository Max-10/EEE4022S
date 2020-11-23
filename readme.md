Initialized by Azure Data Factory!
These are ETL pipelines designed for two weight and tag log data files generated at a remote weighbridge deployment at a penguin colony. The tag log files contained debug information, in addition to the tag number and timestamp of a tagged bird crossing the perimeter. The weightlog file contained estimated weights and timestamps for weighbridge crossings, as well as incorrect readings.
These pipelines extract these dat, process them(filter out readings, create date/time columns, generate primarykey) and upsert them into the relevent table in a sql database.
