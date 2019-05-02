# Using Watson Assistant to perform Long Tail Search in Watson Discovery

In Watson Assistant Plus/Premium, there are two skills. A dialog skill and a search skill. The dialog skill is what was previously known as short tail search. The search skill now provides a means of performing a long tail search using Watson Discovery integration. 


- Short tail: Explicit responses that you provide to the most frequently asked questions (within the dialog skill).<br>

- Long tail: Provides relevant links to content when dialog nodes do not match the user’s question, can be achieved with the                      "if anything else/search skill trigger" https://cloud.ibm.com/docs/services/assistant?topic=assistant-skill-search-add or an explicit call to do a search on a subset of documents triggering on a specific entity e.g. product


Pre-requisites:
IAM must be set up before:
- Provisioning a new instance of Watson Assistant Plus/Premium 
- Upgrading to the Plus/Premium plans on a Cloud Foundry Watson Assistant service
