---
layout: post
title: "Microsoft Azure: Fundamentals and Core Services (Part 1)"
date: 2025-08-22
---

## Introduction

Greetings and welcome to the first article in an exciting new series. In this article, we’ll be talking about Microsoft, its cloud computing platform, some technical explanations, and the development of a culture that you’ll carry with you throughout all of my future blog posts. If you know Microsoft, then you surely know the company’s cloud computing platform. I’m talking about Azure. To ensure you fully grasp the purpose of these articles, know that every explanation will be as in-depth and detailed as possible to enable complete understanding.

Concretely, Microsoft Azure is a hyperscale public cloud built on a global network of interconnected data centers. A hyperscale public cloud refers to a public cloud infrastructure operated by a provider that can deploy computing resources on a massive scale, in a highly automated and elastic way. In short, it’s essentially a public cloud, accessible to anyone, operating at an almost worldwide scale. In the context of cloud computing platforms such as Microsoft Azure, we’ll be talking about terms like services and even resources.

> Moreover, it’s important to know that there are several well-known cloud computing platforms provided by equally well-known multinational companies. For example, there’s AWS (Amazon Web Services) from Amazon, and there’s also GCP (Google Cloud Platform), which is Google’s official cloud computing platform.

To fully understand what Microsoft Azure is, and to avoid throwing around terms like "Cloud Computing" or "Services" without explanation, I’ll provide some clarity. A cloud computing platform is a software abstraction layer that orchestrates, exposes, and delivers virtualized and distributed computing resources over a network (most often the Internet), following standardized service models ([IaaS](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-iaas), [PaaS](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-paas), [SaaS](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-saas)). In fact, public cloud platforms such as AWS, GCP, or Microsoft Azure are generally deployed over the Internet to ensure proper accessibility.

Concretely, cloud computing service models represent the different ways a cloud provider makes its resources available to users. Each model corresponds to a different level of abstraction and defines how responsibilities are divided between the provider and the client. The three most well-known models are IaaS, PaaS, and SaaS, with more specialized variations such as [FaaS](https://www.ibm.com/think/topics/faas), [CaaS](https://www.ibm.com/think/topics/containers-as-a-service), or [DBaaS](https://www.ibm.com/think/topics/dbaas).

![image](https://saberda.github.io/2017/09/28/Cloud-Service-Models/1.png)

Indeed, cloud computing service models are organized along a continuum where technical responsibility gradually shifts from the client to the provider. With IaaS, the client retains significant control but also greater responsibility. With PaaS, the focus is mainly on code and data. With SaaS, users consume ready-to-use applications directly. Modern variants such as FaaS or DBaaS push this abstraction even further, allowing companies to concentrate solely on their core business value.

At the very beginning, with its official launch in 2010, Windows Azure (the former name of Microsoft Azure) primarily offered a PaaS (Platform as a Service) model. Microsoft’s initial idea was not to compete directly with AWS on infrastructure (IaaS), but rather to provide an integrated platform for .NET developers. The first available services were therefore focused on developing and hosting applications in the cloud, without customers having to manage virtual machines or operating systems themselves. Among these were Windows Azure Compute (for hosting applications), SQL Azure (a managed relational database), along with storage and messaging services.

> For info, it was only from 2012 onward that Microsoft expanded Azure into an IaaS model, introducing virtual machines and virtual networking to meet market demand and compete more directly with AWS. Feel free to visit Microsoft’s TechCommunity section, where you can read an [article](https://techcommunity.microsoft.com/blog/educatordeveloperblog/the-history-of-microsoft-azure/3574204) discussing the history of Microsoft Azure.

Today, Azure brings together more than 200 cloud products and services, covering a wide range of needs: machine learning solutions, Internet of Things (IoT) platforms, DevOps tools, advanced security services, relational and NoSQL databases, as well as hybrid and multicloud environments. This diversity allows Azure to serve both startups and large enterprises, offering building blocks tailored to their digital transformation.

Microsoft also highlights the trust that major companies place in Azure: according to the company, 95% of Fortune 500 businesses use the platform for their cloud services. This massive adoption illustrates Azure’s reliability, functional richness, and ability to meet critical challenges, whether in performance, security, or regulatory compliance. By combining a complete ecosystem with large-scale adoption, Azure has established itself as an essential global player in cloud computing.

## Services

## Writing...
