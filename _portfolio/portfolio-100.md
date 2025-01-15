---
title: "Crop type segmentation with multi-temporal imagery"
excerpt: "This project demonstrates the benefits of multi-temporal data for semantic segmentation of satellite imagery for crop type identification. <br/><img src='/images/results-comparison.png'>"
collection: portfolio
---

This project demonstrates the benefits of multi-temporal data for semantic segmentation of satellite imagery for crop type identification. Because of the seasonal patterns present in crop growth, the use of time series can improve crop type classification results. In this project, I use the frozen pretrained encoder from the [Prithvi](https://huggingface.co/ibm-nasa-geospatial/Prithvi-100M) foundation model and train a segmentation head for this task using Landsat 9 imagery (6 bands) as inputs and the Cropland Data Layer (CDL) as labels. The time series are monthly composites from a region in the Sacramento Valley across the growing season (Feb-Sep) for the year 2022. The multi-temporal model achieves a 47% improvement in performance over mono-temporal.

Sample results:

![results comparision](/images/results-comparison.png)

See the full results and code on [Github](https://github.com/keves1/crop-type-segmentation)
