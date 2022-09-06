# VISUM 

## Background
Visum is a Cost Optimization Tool for Cloud Native Applications. The first version of this project takes a [bottom up](https://en.wikipedia.org/wiki/Top-down_and_bottom-up_design) approach and focuses on cost optimization of [Apache Spark](https://spark.apache.org/) Applications that are running on [AWS](https://en.wikipedia.org/wiki/Amazon_Web_Services/). However, an Apache Spark Application is a private case of Cloud Native Applications. Later, Visum can be extended to handle any Cloud Native Application.

### Apache Spark
[Apache Spark](https://spark.apache.org/) is an open-source unified analytics engine for large-scale data processing. Spark provides an interface for programming clusters with implicit data parallelism and fault tolerance.

<table width="256px">
  <tr>
    <td><img src="./images/spark-1.png"/></td>
  </tr>
  <tr><td align="center">Apache Spark</td></tr>
</table>  

### Apache Spark Applications on Cloud
[ESG research](https://aws.amazon.com/big-data/what-is-spark/) found that 43% of respondents considering cloud as their primary deployment for Apache Spark. And it makes a lot of sense because the cloud provides scalability, reliability, availability, and massive economies of scale. Another strong selling point of cloud deployment is a low barrier of entry in the form of managed services. Each one of the [Big 3](https://www.itprotoday.com/iaas-and-paas/big-3-public-cloud-providers-continue-dominate-led-aws) cloud providers comes with its own offering to run Apache Spark as a managed service. 

### Apache Spark Applications and Cloud Costs
Running high scale Apache Spark Application on Public Clouds is expensive. For example, The Amazon EMR price is added to the price for the underlying servers and Amazon Elastic Block Store (Amazon EBS) price. In simple words, applications are billed for per-second * number of cores + cost of storage + managed service (see EMR) fee.

In terms of performance, there are a lot of things that can potentially go wrong: executors can fail, the latency to external data sources can increase, the performance can degrade because of changes in the nature of the input data or because of code changes, and many more. In order to address all these potential issues, it is necessary to proactively monitor the important metrics in real-time. 





