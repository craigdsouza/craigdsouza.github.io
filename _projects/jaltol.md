---
layout: default
title: "Jaltol"
description: "A tool for water resource tracking and analysis."
date: 2025-05-31
tags: [water, data, open-source, Web App]
image: /img/tools/jaltol.png
---

# Jaltol

![Jaltol](/img/tools/jaltol.png)

A geospatial web app that leverages public satellite imagery for water resources monitoring. Developed by my team and I at WELL Labs, used by hydrologists internally at WELL and by partner organisations for monitoring their field implementation.

## Problem statement
Organisations focused on water conservation in rural India primarily hope that access to water acts as a lever, helping rural communities grow more crops and increase their incomes. Billions of dollars are poured into water conservation schemes each year with this hope. Manual groundtruthing of the outcome is expensive and is only carried out sparsely. Whether or not the outcome was achieved is hard to know for sure. 

## Solution
Jaltol aims to address this problem by enabling annual monitoring of changes in crop cover using public satellite imagery sources. 

## How it works
An orthomosaic (RGB) satellite image is turned into a Land Use Land Cover (LULC) raster map. LULC maps are available for different use cases. The use case Jaltol addresses, requires cropping cover estimates during three agricultural seasons of the year for every pixel in the satellite image. This LULC map, is analysed within a unit of interest (a village boundary vector) to quantify the seasonal changes in cropping year-on-year. Jaltol allows for comparison of these cropping statistics for multiple years for treatment and control villages. The app itself is built on the React Framework, with Fast API for the backend. 


**Links** - [Jaltol Web App](https://jaltol.app/impact-assessment/app)

Github : [Frontend](https://github.com/WELLlabs/JaltolUI) \| [Backend](https://github.com/WELLlabs/JaltolAPI)
