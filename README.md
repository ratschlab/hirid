
# HiRID data

HiRID is a freely accessible critical care dataset containing data from more than 33,000 patient admissions to the Department of Intensive Care Medicine, Bern University Hospital, Switzerland (ICU) from January 2008 to June 2016.
It was first released as part of the [circulatory Early Warning Score](https://www.nature.com/articles/s41591-020-0789-4) project. 

More in detail the documentation contains the following sections of interest:
- [Getting started](https://hirid.intensivecare.ai/getting-started) This first section points to a jupyter notebook to familiarize yourself with the data.
- [Data details](https://hirid.intensivecare.ai/data-details) This second section contains a description of the variables existing in the dataset. To complete this section you can refer to our [varref.tsv](preprocessing/resources/varref.tsv) which we use to build the common version of the data.
- [Structure of the published data](https://hirid.intensivecare.ai/structure-of-the-published-data) This final section contains details about the structure of the raw data you will have to download and place in `hirid-data-root` folder (see "Run Pre-Processing").

## Download Data

1. Get access to the HiRID 1.1.1 dataset on [physionet](https://physionet.org/content/hirid/1.1.1/). This entails
   1. getting a [credentialed physionet account](https://physionet.org/settings/credentialing/)
   2. [submit a usage request](https://physionet.org/request-access/hirid/1.1.1/) to the data depositor
2. Once access is granted, download the following files
   1. [reference_data.tar.gz](https://physionet.org/content/hirid/1.1.1/reference_data.tar.gz)
   2. [observation_tables_parquet.tar.gz](https://physionet.org/content/hirid/1.1.1/raw_stage/observation_tables_parquet.tar.gz)
   3. [pharma_records_parquet.tar.gz](https://physionet.org/content/hirid/1.1.1/raw_stage/pharma_records_parquet.tar.gz)
3. unpack the files into the same directory using e.g. `cat *.tar.gz | tar zxvf - -i`

## License
You can find the license for the original HiRID data [here](https://physionet.org/content/hirid/view-license/1.1.1/).
