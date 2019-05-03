# Using Watson Assistant to perform Long Tail Search in Watson Discovery

## Reasons for Implementing Long Tail Search in Watson Assistant

In Watson Assistant Plus/Premium, there are two skills. A dialog skill and a search skill(beta) currently. Previously, there was only built-in capability for short tail search using the dialog skill. The search skill now provides a means of performing a long tail search using Watson Discovery integration for self-service.More reasons for implementing long tail search in Watson Assistant can be found in this blog: https://medium.com/ibm-watson/adding-search-to-watson-assistant-99e4e81839e5


## Basic Review of Concepts
- Short tail: Explicit responses that you provide to the most frequently asked questions (within the dialog skill).<br>

- Long tail: Provides relevant links to content when dialog nodes do not match the user’s question, can be achieved with the                      "if anything else/search skill trigger" https://cloud.ibm.com/docs/services/assistant?topic=assistant-skill-search-add or an explicit call to do a search on a subset of documents triggering on a specific entity e.g. product


## Pre-requisites:
- IAM must be set up before provisioning a new instance of Watson Assistant Plus/Premium 
- Migration of the Cloud Foundry Watson Assistant service must be completed prior to upgrading to the Plus/Premium and existing Watson Assistant premium customers must migrate to IAM by June 2019. 
  
  
## 3 step process for 
  
  

  
  

