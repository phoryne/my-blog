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

In this section, we will look together at the services Azure offers, the products provided within those services (not all of them, of course), and the key terminologies necessary to understand an Azure architecture. First, it is essential to understand Azure’s overall architecture. This architecture is relatively straightforward. At the top, there is the Azure portal, which is the graphical interface used to manage resources. Beneath it are the services offered by the platform, such as compute, storage, networking, and databases, which we will explore in more detail later. Each service contains different products depending on its category, and from these products, you can deploy and configure resources, such as a virtual machine, an SQL database, or a storage account.

![image](https://i.ibb.co/99Q4JJfJ/image.png)
