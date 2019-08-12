---
title: "Predictive analytics for image super-resolution"
date: 2018-07-14
tags: [Machine Learning]
header:
  overlay_image: "/images/yellow.jpg"
  overlay_filter: 0.2
excerpt: "Carry out model evaluation and selection for predictive analytics on image data"
mathjax: "true"
siderbar:
  title: "Data Science Portfolio"
  nav: sidebar-sample
---
<figure>
<img src="/images/predictive/hr.png">
</figure>
<h1 style="font-family:'Roboto';font-size:18px;">Project summary</h1>
<ul class="thin-text">
<li>In this project, we will carry out model evaluation and selection for predictive analytics on image data. Here we evaluate different modeling/analysis strategies and decide what is the best. And the decisions are supported by sound evidence in the form of model assessment, validation and comparison. Here, PSNR is the key factor we look into.</li>
<li>In addition, we also need to communicate our decision and supporting evidence clearly and convincingly in an accessible fashion. We were given a training set of 3000 images to realize a super resolution algorithm (half LR and half HR).</li>
<li>The baseline model is random feature extraction + GBM model. For improved model, we try different feature extraction methods, such as Canny, diagonal methods. We also try XGBOOST model. Our optimal model is using XGBOOST model on canny features, which leads to 25.23 PSNR, with a test running time of 784 seconds for 1500 images, whereas the baseline model is of 19.07427 PSNR and 2177.6 seconds. </li>
<figure>
  <img src="/images/predictive/flow.png">
</figure>
<li>Additionally, we use deep convolution neural network to evaluate the prediction analysis and obtain a PSNR of around 50 and a consuming time of around 45 minutes, but it did not satisfy the requirement of expanding image dimension. Thus, we choose not to use that model here.</li>
</ul>
<br>
<h1 style="font-family:'Roboto';font-size:18px;">Contribution Statement</h1>
<div style="font-size:14px;font-family:'Montserrat';text-indent:20px;">
All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement.
</div>
<ul class="thin-text">
<li><strong>Yang Cai:</strong> is responsible for constructing the features and developing the GBM model.</li>
<li><strong>Yang Chen:</strong> Built baseline model(GBM). Evaluate model with SR-CNN Tensorflow. Updated the Summary section in the Readme file of the project. Prepare for this project from the group.</li>
<li><strong>Yiming Shi:</strong> is responsible for constructing the features and developing the GBM model.</li>
<li><strong>Kehui Zhu:</strong> is responsible for constructing the features and developing the GBM model.</li>
<li><strong>Siyu Zhu:</strong> Main contributor to the baseline model (completed the feature.R and superResolution.R) and Optimal model(XGBoost model). Responsible for GBM and XGBoost models' parameters tuning. Assist with the SRCNN model's implementation.</li>
</ul>
<br>
<h1 style="font-family:'Roboto';font-size:18px;">References</h1>
<ol class="thin-text">
<li><a href="https://rpubs.com/mharris/multiclass_xgboost">https://rpubs.com/mharris/multiclass_xgboost</a>: Perform XGBoost</li>
<li><a href="http://www.milanor.net/blog/cross-validation-for-predictive-analytics-using-r/ ">http://www.milanor.net/blog/cross-validation-for-predictive-analytics-using-r/ </a>: CV error</li>
<li><a href="https://cran.r-project.org/web/packages/gbm/gbm.pdf">https://cran.r-project.org/web/packages/gbm/gbm.pdf</a>,<a href="https://github.com/TZstatsADS/Fall2017-project3-grp3">https://github.com/TZstatsADS/Fall2017-project3-grp3</a>: Perform GBM</li>
<li><a href="https://github.com/tegg89/SRCNN-Tensorflow">https://github.com/tegg89/SRCNN-Tensorflow</a>: SRCNN</li>
</ol>
<br>
<h2 class="thin-text">You can find the code of this project <a href="https://github.com/TZstatsADS/Fall2018-Proj3-Sec2-grp2.git">here</a>.</h2>
