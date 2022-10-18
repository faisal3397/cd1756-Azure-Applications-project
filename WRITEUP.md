# Solutions Comparison & Analysis
<br>

### Analyze, choose, and justify the appropriate resource option for deploying the app.

<br>
<!-- *For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice* -->

----------------------------


## **Cost**:

### **VM**:
The **Bs-series**, which is the economical choice Could range from **$3.7/month** to **$607.3/month**.
### **App Service**:
The **Pay as you go price** Could range from **Free** to **$219/month**

### **Reference**:

https://azure.microsoft.com/en-us/pricing/details/virtual-machines/linux/#pricing

https://azure.microsoft.com/en-us/pricing/details/app-service/windows/

----------------------------

## **Scalability**:
### **VM**:
Could be done using [**Virtual Machine Scale Sets**](https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview), which will allow your application to scale depending on the demands
### **App Service**:
It's already built to ease up the process of scaling up your application. Also, it has the feature of auto-scaling.

### **Reference**:

https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview

https://learn.microsoft.com/en-us/azure/app-service/manage-scale-up

----------------------------


## **Availability**:
### **VM**:
Test
### **App Service**:
Test

----------------------------


## **Workflow**:
### **VM**:
VM's workflow requires extra steps in order for you to deploy, it will require you to copy the project to the VM's instance, and any change that you do to the application will require the same steps of copying the project to the VM.
### **App Service**:
App Service's workflow to deploy an application is much simpler than the VM, as it will only require you to link it to the project's repo with specifying your main branch, and with any push to that branch, the pipeline will immediately trigger to deploy your changes

----------------------------
## Choice: **App Service**
<br>

## **Justification**:

As the application is simple and lightweight, and I don't need any control over the OS or the VM's resources, I chose the App Service as it will fit the current project's need efficiently.

----------------------------
## Assess app changes that would change your decision.
<br>
<!-- *Detail how the app and any other needs would have to change for you to change your decision in the last section.*  -->

In case I had to be in control over the OS or the app environment, or in case the application required dedicated servers for security or other reasons, then I'll change my decision and go with the VM.