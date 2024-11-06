---
{"dg-publish":true,"permalink":"/thibs-corner/customer-stories/2014-arkema-smart-batch-monitoring-with-vba-improves-problem-identification/"}
---

[Company:: Arkema]
[Industry:: #Industry/Chemicals]
[Year:: 2014]
[Title:: [Smart Batch Monitoring with VBA Improves Problem Identification](https://resources.osisoft.com/presentations/smart-batch-monitoring-with-vba-improves-problem-identification/)]
[PDF:: [PDF](https://cdn.osisoft.com/corp/en/media/presentations/2014/UsersConference2014/PDF/UC2014_Arkema_Duffy_SmartBatchMonitoringwithVBAImprovesProblemIdentification.pdf)]
[Country:: France]
[Products:: [[Product\|Product]]]
[Business Impacts:: #BusinessImpact/EventFrames/GoldenBatch]
  

---
## Arkema's Results
![](https://i.imgur.com/pJOsTwU.png)
![](https://i.imgur.com/eDonHNa.png)
![](https://i.imgur.com/LKhE6hm.png)
![](https://i.imgur.com/XxzjctG.png)
![](https://i.imgur.com/dVMUGwU.png)
![](https://i.imgur.com/XAZ9gBc.png)
![](https://i.imgur.com/Tmwqa5U.png)
![](https://i.imgur.com/K2kPQnA.png)---
## Screenshots

---
## Description
Smart batch monitoring is an effective way to easily identify problems as they occur, and provides engineering and operations valuable time to react to the batch and prevent the problem from propagating into more problems downstream, as well as to provide better visibility for predictive scheduling. Trending problems can also identify necessary maintenance work while the problem is minor, allowing maintenance work to be done on schedule and before major failures. This concept is useful for almost any operation, but is especially useful in batch plants with numerous different recipes which it would be unrealistic to update manually.

The PI ProcessBook display uses PI Batch and visual basic coding to show characteristic trends, such as temperature, pressure, progression of reaction, and steam usage, for each batch currently being produced. These trends are overlaid on the recent history of this product’s production in this vessel using a batch group, and then have a “golden batch” identified by engineering added to the batch group using Visual Basic (VB). Small deviations such as temperature or a higher than normal steam usage can be indications of a problem such as contamination, off-track reactions, and equipment fouling or fatigue; this display makes these deviations obvious. The use of VB coding allows the display to run untouched in the control rooms 24/7 with operators able to constantly monitor the batches at a level of detail necessary to reliably and quickly identify problems while they are still small. The code refreshes the display every time a new recipe is set to a production vessel in the DCS by changing the product being displayed to match the one that is now being made, and changes the golden batch to this product’s ideal instance.