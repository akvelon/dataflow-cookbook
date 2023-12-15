# Read and Write TFRecord Files with Apache Beam

This folder contains code that demonstrates how to read / write data in TFRecord format using Apache Beam.

## Execution Instructions

### Prerequisites

- Python 3.x installed
- Apache Beam library installed (`pip install apache-beam`)

### Steps for running Read example

1.**Create set of .tfrecord files.**

2.**Run the code:**

Execute the script `read_tfrecord.py` with the following parameters:

```
python read_tfrecord.py --runner="DataflowRunner" --project="your-project" --region="your-region" --file_pattern="your-file-pattern"
```

- `--runner`: Specify the Apache Beam runner (here, `DataflowRunner` is used).
- `--project`: Provide your Google Cloud project ID.
- `--region`: Specify the region where the Dataflow job will run.
- `--file_pattern`: Set the file pattern for the TFRecord files.

### Steps for running Write example

1.**Create a folder for TFRecord files:**

Create a folder where the generated TFRecord files will be stored.

2.**Run the code:**

Execute the script `write_tfrecord.py` with the following parameters:

```
python write_tfrecord.py --runner="DataflowRunner" --project="your-project" --region="your-region" --file_path_prefix="your-file-path-prefix"
```

- `--runner`: Specify the Apache Beam runner (here, `DataflowRunner` is used).
- `--project`: Provide your Google Cloud project ID.
- `--region`: Specify the region where the Dataflow job will run.
- `--file_path_prefix`: Set the file path prefix for the TFRecord files.


## Additional Information

### References

For more information on Apache Beam and TFRecord:

- [Apache Beam Documentation](https://beam.apache.org/documentation/)
- [TFRecord Documentation](https://www.tensorflow.org/tutorials/load_data/tfrecord)