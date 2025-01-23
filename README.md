## Achieving Efficient and Accurate Privacy-Preserving Localization for Internet of Things: A Quantization-Based Approach
## Description
This is the official implementation for our paper [Achieving Efficient and Accurate Privacy-Preserving Localization for Internet of Things: A Quantization-Based Approach]. 
## Abstract
Privacy-preserving localization is an important enabling technology for location-based applications on the Internet of Things (IoT). Existing work utilizes encryption or noise-adding mechanism to develop privacy-preserving methods during the localization process. However, these methods still face the challenge of simultaneously achieve localization accuracy, privacy preservation and communication efficiency. To address the challenge, in this paper, a novel quantization-based privacy-preserving localization (QPPL) algorithm is proposed to estimate the target’s location with accuracy, privacy preservation and communication efficiency at the same time. Firstly, the location information is quantized, i.e., deviate the location data, to preserve the private location information during the localization process. With the quantization on the location information, the data scale is compressed to reduce communication cost and improve localization efficiency. Then, to improve the localization accuracy, an optimal weight allocation scheme is designed to aggregate the location estimates from the heterogenous anchor devices. By minimizing the weighted sum of squared quantization errors of all anchor devices, a closed form optimal weight allocation scheme is derived by using convex optimization theory. Finally, through theoretical analysis, we prove the accuracy, privacy preservation and efficiency of the QPPL algorithm. Experimental evaluation demonstrates that QPPL has superior performance compared with existing methods.
## MATLAB Implementation
-Localization algorithm.
 
    ProposedLocAlgorithm.m, PPProposedLocAlgorithm.m, GPPADL.m, HPPL.zip
  
-Quantization.
 
    quantize_clipping.m

-The influence of the number of iterations on localization error and the weighted sum of SQE.
  
    Test_Iterations.m, Test_SQE.m

-The localization error with the number of anchors and the number of measurements.
  
    Test_AnchorNumber.m, Test_Measurement.m

-The influence of the quantization accuracy on localization error.
  
    Test_Diffbits.m

-The influence of the number of anchors on communication overhead and the running time.
  
    Test_Time.m, Test_Cost.m

-The localization error with the number of misbehaving anchors.
  
    Test_Misbehaving.m

-The influence of region size on localization error.
  
    Test_Biggerarea.m, Test_Gdop.m

-The influence of the distribution of anchors on the localization error.
  
    Point_tri.m, Test_Tri.m

-The localization error in dynamic networks.
  
    Test_Dynamic.m
