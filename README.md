# LLGS: Illuminating Gaussian Splatting via absorptance Modulation

# Ablation Study of Absorption Modulation

This section presents the ablation experimental results of our absorption modulation method. In this experiment, we removed the MLP network that calculates the absorption coefficient theta and added absorption coefficients to the Gaussian. Then, we directly calculated the gradient of theta during the backpropagation stage of Gaussian scattering, and updated the value of theta. The other settings are the same as our method, and the following are the experimental results on buu dataset.
![fig1]([fig1.png](https://github.com/LLGS2024/LLGS/blob/main/fig/fig1.png))
The experimental results depicted in Figure 1 illustrate that, in the absence of our absorption model, the updating process of the absorption coefficient fails to effectively capture the color and structural information of the scene. This leads to the rendered images exhibiting dark shadows and a hazy appearance, which significantly compromises the integrity of the image structure and hinders the accurate acquisition of detailed scene information. Conversely, our absorption model, which is formulated based on the Lambert-Beer law, thoroughly considers the color information and scene structure, playing a vital role in the rendering outcome.


# Real-world Low Light Scene Testing

Description of section 2.
