---
layout: post
title: "Microsoft Azure: Fundamentals and Core Services (Part 1)"
date: 2025-08-22
---

## Introduction

Hey, for my first article, I wanted to start with a series of articles that I’ve been passionate about for quite some time now. This article marks the beginning of a long series on the study of Microsoft Azure, Microsoft’s cloud computing platform. For this first article, we’ll take a global look at what Microsoft Azure is and the world of cloud environments. Why? Well, because in future articles, I’ll dive deeper into certain concepts related to Azure, across different domains, in a detailed and technical way. This is one of the reasons why I suggest you make sure to properly understand all the concepts in this article. Without them, you may have trouble following the rest of the series (unless you’re already a Microsoft expert). I hope you’ll enjoy it and, without further ado, let’s get started.

Before we begin, I need to give you a quick heads-up. In this article, we’ll only be covering topics directly related to Microsoft Azure. Therefore, I suggest you at least have some basic knowledge and understanding of what cloud computing platforms are (since this is not the central focus of the article), how they work, and some familiarity with the related concepts.

## What is Microsoft Azure?

Microsoft Azure, formerly known as Windows Azure, is a cloud computing platform developed by Microsoft. It was officially announced in October 2008 under the name Windows Azure during the Microsoft Professional Developers Conference (PDC). The platform was later made publicly available in February 2010. In March 2014, Windows Azure was renamed Microsoft Azure, to reflect its broader focus beyond Windows and toward a more comprehensive cloud offering. If you happen to be living in a cave, reading this article on a scrap of paper, without internet access, and without having kidnapped a Microsoft employee to keep you company, the project’s logo looks like a stylized light-blue "A". There are other well-known cloud computing platforms as well. To give you an idea, there’s AWS (Amazon Web Services) from Amazon, GCP (Google Cloud Platform) from Google, and Azure from Microsoft. All three solutions offer more or less the same types of services and work in roughly the same way, the main difference being that they come from three different companies.

What is interesting to know are the figures provided by Microsoft. They actually offer more than 200 products spread across their available services.  
We will have the opportunity to discuss this later in the article. Below, you can see an overview of the products offered, spread across Microsoft’s broad service categories.

![image](https://pmss.ms/img/azure-1.jpg)

Moreover, they claim to provide their services to over 95% of the Fortune 500 multinational companies. What Microsoft Azure offers is a solution that enables companies using its various services to migrate from their on-premises infrastructures to fully cloud-based solutions, or to hybrid infrastructures (cloud + on-premises).

Speaking of numbers, Microsoft operates more than 400 highly secure data centers across over 70 regions. Thanks to this, Azure provides the broadest cloud footprint, giving businesses more regions to choose from than any other cloud provider. In fact, businesses of all sizes rely on Azure to help them bring their ideas to life, seamlessly unify their technology, and innovate with confidence. One thing that caught my attention and that I find interesting is that Azure offers built-in security solutions designed to protect business workloads, from code to cloud. 

When talking about cloud solutions, one cannot overlook Artificial Intelligence. Azure AI Foundry provides an end-to-end AI platform, encompassing models, tools, security features, and monitoring capabilities to help organizations design and scale their AI applications efficiently and cost-effectively. A global overview of the solution is shown below.

![image](https://devblogs.microsoft.com/foundry/wp-content/uploads/sites/89/2025/03/foundry-stack-wp-2048x1152.png)

In fact, Azure AI Foundry’s models include more than 11,000 options, giving organizations unmatched flexibility to choose and build AI solutions tailored to their needs.

One of the reasons organizations use Microsoft Azure as their cloud computing solution is that a dedicated team of more than 10,000 security experts continuously monitors systems, detects vulnerabilities, and tracks breach patterns as well as malicious actors. The team synthesizes 78 trillion security signals every day using AI and advanced analytics to understand and defend against cyber threats. Microsoft reinforces this commitment with a planned investment of USD 20 billion in security over the next five years.

Currently, Microsoft Azure offers several types of cloud service models. Notably, they provide IaaS (Infrastructure as a Service), PaaS (Platform as a Service), SaaS (Software as a Service), AIaaS (Artificial Intelligence as a Service), and MaaS (Models as a Service). This offers a comprehensive range of options for all types of organizations.

## Services, Products & Resources

In this section, we will look together at the services Azure offers, the products provided within those services (not all of them, of course), and the key terminologies necessary to understand an Azure architecture. First, it is essential to understand Azure’s overall architecture. This architecture is relatively straightforward. At the top, there is the Azure portal, which is the graphical interface used to manage resources. Beneath it are the services offered by the platform, such as compute, storage, networking, and databases, which we will explore in more detail later. Each service contains different products depending on its category, and from these products, you can deploy and configure resources, such as a virtual machine, an SQL database, or a storage account. Below is an image of some of the products and services offered by Microsoft Azure.

![image](https://eu-images.contentstack.com/v3/assets/blt07f68461ccd75245/blt631316163dc18945/66180d2ac88264e5cce39ec5/azureresourcesmaphero_0_4.png?width=1280&auto=webp&quality=80&format=jpg&disable=upscale)

Now, here’s where things get a bit more technical.  

A **service** in Azure is a family of capabilities (e.g., Compute, Storage, Networking, Databases). Each service exposes **resource types** through what is called a **resource provider** (for example: `Microsoft.Compute/virtualMachines`, `Microsoft.Storage/storageAccounts`). A **product** or **SKU** is a variant of a resource type with specific features and a specific pricing model (for instance, a VM size like `Standard_D2s_v5` or a Load Balancer tier such as Basic vs. Standard). Finally, a **resource** is the actual instance you create in your subscription (e.g., a VM named `myVM01` deployed in France Central).

Azure resources are organized in a hierarchy:  
- At the top, you have a **Microsoft Entra ID tenant** (identity directory).  
- Then, **management groups** (optional), used to organize and apply policies across multiple subscriptions.  
- **Subscriptions**, which are billing and security boundaries.  
- **Resource groups**, logical containers for resources that share the same lifecycle.  
- **Resources**, the deployed instances (VMs, databases, storage accounts, etc.).  

Every resource has a unique **resource ID**, and permissions are managed using **RBAC** (Role-Based Access Control) that can be applied at any level (management group, subscription, resource group, resource).

Azure also operates across **regions** (sets of data centers) and **availability zones** (isolated data centers within a region). Some regions are paired with others to improve disaster recovery. Not all services or SKUs are available in all regions, so when you create a resource, you must check the availability.

On top of this, Azure offers strong **governance tools**:  
- **Tags** (key-value pairs) to organize resources and track costs.  
- **Locks** (`CanNotDelete` or `ReadOnly`) to protect critical resources from accidental changes.  
- **Azure Policy** to enforce compliance (e.g., require encryption, restrict regions, or audit resource configurations).  
- **Deployment Stacks** (the successor of Blueprints) to manage infrastructure deployments at scale.

For **automation and Infrastructure as Code (IaC)**, Azure uses **Bicep** (a modern declarative language) and ARM templates (JSON). You can deploy in *incremental* mode (recommended, only adds/updates resources) or *complete* mode (which deletes what’s not in the template). Features like **what-if deployments** help preview changes before applying them.

On the **identity side**, Azure integrates with Microsoft Entra ID. You can assign roles via RBAC and use **Managed Identities** to let applications access Azure resources securely without storing secrets.

From a **billing perspective**, each subscription is linked to a billing account, and every resource consumes **billing meters** (units of usage, e.g., hours, GB). Costs vary by **SKU**, **region**, and consumption. Azure also provides **Reservations** and **Savings Plans**: by committing to a specific service (e.g., VMs, SQL databases, storage) for one or three years, organizations can achieve significant discounts.

Finally, Azure includes the **Marketplace**, which offers third-party and Microsoft-published solutions (VM images, SaaS apps, managed services). Each Marketplace offer has **plans** (similar to SKUs) with different features and prices.

### A concrete example:
Let’s say you need a virtual machine. You select the **Compute service**, then choose the **resource type** `virtualMachines` from the provider `Microsoft.Compute`. You pick a **SKU** (say, `Standard_D4s_v5`), deploy it in a **resource group** inside the **France Central region**, and Azure creates a **resource**. That VM consumes billing meters (compute hours, disks, network), can be tagged (`CostCenter=Finance`), secured with RBAC and locks, and monitored through Policy. If you know you’ll use it for the next three years, you could apply a **reservation** to reduce costs.

This layered model—**services → SKUs/products → resources → governance & billing**—is the foundation of Azure’s architecture. Once you understand it, everything else (from AI services to networking) falls naturally into place.
