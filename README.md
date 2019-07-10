# ENTRADA

ENTRADA - A big data tool for network analytics.

Convert and enrich network data in PCAP format to Apache Parquet format and send the results to any of these endpoints: 
- HDFS + Impala (hadoop)
- S3 + Athena (aws)
- Local disk (local)

Apache Impala, AWS Athena or Apache Spark can be used to analyse the generated Parquet data.  

ENTRADA handles the required workflow actions such as:  
- Loading and archiving PCAP files
- Converting and enriching data
- Creating database schema and tables
- Creating a S3 bucket
- Configuring S3 security policy and encryption
- Creating filesystem directories
- Moving data files around
- Uploading data to HDFS or S3
- Compacting Parquet files on HDFS or S3

For more information see the [ENTRADA wiki](https://github.com/SIDN/entrada/wiki).

## How to use

ENTRADA can be deployed using Docker, pull the docker image from Docker hub.  

```
   docker pull sidnlabs/entrada:<tag>

```

Download one of the example [Docker Compose scripts](https://github.com/SIDN/entrada/tree/master/docker-compose)  
Modify the environment variables for hostnames and filesystem paths to fit your requirements and then start the container.  


```
   docker-compose up -d

```


For more information about deployment and available onfiguration options see the [ENTRADA wiki](https://github.com/SIDN/entrada/wiki/).  

## License

This project is distributed under the LGPL, see [LICENSE](LICENSE).

## Attribution

When building a product or service using ENTRADA, we kindly request that you include the following attribution text in all advertising and documentation.
```
This product includes ENTRADA created by <a href="https://www.sidnlabs.nl">SIDN Labs</a>, available from
<a href="http://entrada.sidnlabs.nl">http://entrada.sidnlabs.nl</a>.
```
