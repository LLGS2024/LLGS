# LLGS: Illuminating Gaussian Splatting via absorptance Modulation

# Ablation Study of Absorption Modulation

This section presents the ablation experimental results of our absorption modulation method. In this experiment, we removed the MLP network that calculates the absorption coefficient theta and added absorption coefficients to the Gaussian. Then, we directly calculated the gradient of theta during the backpropagation stage of Gaussian scattering, and updated the value of theta. The other settings are the same as our method, and the following are the experimental results on buu dataset.
<!-- ![本地图片](p1.JPG) ![本地图片](p10.JPG) ![本地图片](p17.JPG)
![本地图片](1.JPG) ![本地图片](10.JPG) ![本地图片](17.JPG) -->
![本地图片](fig1.png)
如图1所示的实验结果显示，失去我们的吸收模型后，由于不能很好地学习到场景的颜色信息与结构信息，导致场景的渲染结果出现黑影与灰雾，严重地破坏了图片的结构，导致无法很好地学习场景的细节信息。相反地，我们的吸收模型基于朗博比尔定律进行建模，充分考虑了颜色信息与场景结构，对于渲染结果有着重要的作用。

# Real-world Low Light Scene Testing

Description of section 2.