# Tutorials and Walkthroughs

## Elasticsearch Tutorials

I'm creating a few tutorials for ElasticSearch to support some of the things I'm working on.  This page is somewhat spartan as I build out the library a bit.

[Creating a Simple ElasticSearch Cluster with VirtualBox](./VBoxESCluster/) covers creating Virtual Machines in VirtualBox, Installing Linux, Configuring Networking and Installing ElasticSearch. This will get a basic three-node cluster up and running for you to experiment with the basics of Elastic.

[Using Nginx to add security to ElasticSearch](./ESwithNginx/) covers installing and configuring Nginx on one of our previously configured VMs to act as a security gateway, a load balancer, or SSL endpoint for ElasticSearch.

[Creating Kibana Visualizations with Bike Share Data](./BikeDataViz/) will use some public bike share data to create a few visualizations with Kibana.  This will be a multi-part walkthrough of creating an index mapping, ingesting data, configuring an index pattern, and data discovery.  It is based on a presentation that I put together for [RocDev](https://rocdev.org/) in December 2019.