# Using Watson Assistant to perform Long Tail Search in Watson Discovery

## Reasons for Implementing Long Tail Search in Watson Assistant

In Watson Assistant Plus/Premium, there are two skills. A dialog skill and a search skill(beta) currently. Previously, there was only built-in capability for short tail search using the dialog skill. The search skill now provides a means of performing a long tail search using Watson Discovery integration for self-service.More reasons for implementing long tail search in Watson Assistant can be found in this [blog:](https://medium.com/ibm-watson/adding-search-to-watson-assistant-99e4e81839e5) 


## Basic Review of Concepts
- Short tail: Explicit responses that you provide to the most frequently asked questions (within the dialog skill).<br>
- Long tail: Provides relevant links to content when dialog nodes do not match the user’s question, can be achieved with the                       ["if anything else/search skill trigger"](https://cloud.ibm.com/docs/services/assistant?topic=assistant-skill-search-add)  or an explicit call to do a search on a subset of documents triggering on a specific entity e.g. product


## Pre-requisites:
- IAM must be set up before provisioning a new instance of Watson Assistant Plus/Premium and Watson Discovery
- Migration of the Cloud Foundry Watson Assistant/Watson Discovery service must be completed prior to upgrading to the Plus/Premium and existing Watson Assistant premium customers must [migrate to IAM](https://github.com/bmguillo/IAM_Tutorial)  by June 2019. 

  
  
## 5 step tutorial for setting up long tail search


### Step1 [Create an Assistant](https://cloud.ibm.com/docs/services/assistant?topic=assistant-assistant-add)  

### Step2  [Create your skill(s)](https://cloud.ibm.com/docs/services/assistant?topic=assistant-skill-add)  

### Step3 [Connect to Discovery](https://www.youtube.com/watch?v=PxGzh2VrCb4&feature=youtu.be)
* Connect to an Existing Watson Discovery Service and Existing Collection(Data Source connection or document upload) or Create new Collection
* Choose carefully the content you upload and quantity
* Provision a new instance of Watson Discovery and Create Data Collection(Data Source connection or document upload) 

### Step4 Finish Setup in Watson Assistant/Configure App in Watson Assistant options within Watson Discovery 
- Configure messages to display when results are returned or not returned
- Map field in our collection with fields we want to display in our chat window e.g. title--> extracted_metadata.title & body--> text
  
### Step5 Test out your search using the try it out feature
- Modify & test until reach results expected
- Exit try it out & click save



### Other Development Considerations
- [Development process:](https://cloud.ibm.com/docs/services/assistant?topic=assistant-dev-process)
- [Creation of skill versions](https://cloud.ibm.com/docs/services/assistant?topic=assistant-versions)
- [Improvement via active interactions with assistant](https://cloud.ibm.com/docs/services/assistant?topic=assistant-logs#logs-deploy-id)
-![Continuous Improvement](https://github.com/bmguillo/WatsonAssistant_SearchSkill/blob/master/Watson%20Assistant%20Continous%20Improvement%20ML%20Best%20Practices%202.pdf)
- [Faster training](https://medium.com/ibm-watson/let-watson-train-your-virtual-assistant-57bd53b12bc3)

  

  
  

