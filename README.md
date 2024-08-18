# Terraform-with-GCP-Learning-Project
Terraform with GCP Learning Project


**This project was done by following a tutorial from FreeCodeCamp**


I was able to apply the concepts here to a domain that I own (maxshaw.online) and create 9 different resources that were deployed to GCP and I was able to reach the domain name with a simple index.html file to display text by using a URL.

I created a DNS zone in GCP called terraform-gcp and set the DNS name to test.maxshaw.online.

To ensure the DNS would map requests properly, I created 4 NS records with my domain provider that referenced the 4 routes created by default when making a DNS zone in GCP. Since the DNS name was test.maxshaw.online it was as simple as creating the NS record with the "host" set to test and the nameserver set to the 4 routes respectively.

I was able to map the domain into this Terraform project by referencing the zone I created in GCP in the main.tf file in lines 31-33
