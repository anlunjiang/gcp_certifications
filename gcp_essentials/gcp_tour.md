# Tour of GCP Platform

## Google Cloud platform console
Central dev hub of most projects - includes web console and status dashboard. Uses include:
* Enabling APIs for a projects
* Creating and deleting buckets
* Uploading, Downloading and Deleting Projects
* Managing IAM Policies

 Access the Console by either clicking on the shell icon within the dashboard or going to: https://console.cloud.google.com/

 Consoles with Bucket only access can be assigned to non project members - able to work only with objects within that bucket: https://console.cloud.google.com/storage/browser/[BUCKET_NAME]

 Like with Buckets, Object only console links exist - which can differ in format depending on the permissions of that object. Public links look like:
 https://console.cloud.google.com/storage/browser/_details/[BUCKET_NAME]/[OBJECT_NAME]

 ## Storage

 **GCP uses a flat namespace to store data**: However cloud console can mimic a folder hierarchy for familiarity
 object naming follows hierarchy, but not actual hierarchy is implemented

 ## Projects
 An organising entity: containing resources and services; pool of VMs, databases and a network. GCP project_id's are globally unique
 > Resources:  
 Physical assets, computers, hard drives, VMs, contained in data centers
 Each data center location is in a **Region** which contains **Zones**
 *  For example, zone a in the East Asia region is named asia-east1-a.
 * Distribution of resources help with redundancy for failure and latency for customers

**Global Resources** - Can be accessed globally - preconfigured disk images, snapshots
**Regional Resources** - Accessed only in the same Region, include static external IP addresses 
**Zonal Resources** - VM Instances, types and disks

> Services: Hardware and Software products in GCP are now services that are provided
* **Compute**: houses a variety of machine types that support any type of workload. The different computing options let you decide how 
* **involved** you want to be with operational details and infrastructure amongst other things.
* **Storage**: data storage and database options for structured or unstructured, relational or non relational data.
* **Networking**: services that balance application traffic and provision security rules amongst other things.
* **Stackdriver**: a suite of cross-cloud logging, monitoring, trace, and other service reliability tools.
* **Tools**: services for developers managing deployments and application build pipelines.
* **Big** Data: services that allow you to process and analyze large datasets.
* **Artificial Intelligence**: a suite of APIs that run specific artificial intelligence and machine learning tasks on the Google Cloud platform.


## Ways to interact with services and resources
* Google Cloud Console
* CLI - Cloud Shell is an in-browser command prompt execution environment to manage resources and services in your GCP project.
* Client Libraries - API

