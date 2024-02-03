
# 🚀 Lab 03- Release Management

## 🎯 Objective
Get hands-on experience with Helm's Function capabilities.

estimated time: 10m

In this Tutorial we are going to have a basic look on how function works and what are the benefits of using them.

## 📚 Instructions

## 1️⃣ Step1 : Inspect the existing Chart

1. Cd to Lab03 and open the existing "Video" chart with visual studio code.

2. We are going to change the file called _helpers.tpl which holds the function definitions.

3. By using your amazing Reverse Engineering skils , Google , Helm Docs and Co-Pilot , perform the following :

- on deployment.yaml line 31 add the container security context from the values file. 
- add a function called "video.image" that is concating the ACR name (Values.acr) the image name and the appVersion of the chart
e.g "vicorpacr.azurecr.io"/indexing-service:1.16.0"

**_NOTE:_** the places to change / add code are marked with +++ADD_CODE_HERE+++

4. Run the template in Lint Mode to ensure it is not missing values and/or has the right allignments.

```bash
helm lint video
```
