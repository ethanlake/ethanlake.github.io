---
layout: default
title: "TLV"
---

# Gradients and Reverse SDEs

## Reverse SDEs

Consider the SDE 
$$ dx = f(t) dt + g(t) dw$$
where $w$ is a standard.


We claim that the reverse SDE is 
$$ dx = [f(t) - g^2(t)\nabla_x\log q_t(x)]dt + g(t) dw$$  
where $dt$ now represents a negative time increment.  

### Derivation 

The modification of the drift term becomes natural if one recalls the derivation of the Fokker-Planck equation. 
We know the marginals $q(x_t | x_{t-1})$ 

## Diffusion Models

The marginals are usually taken to be given by convolution with Gaussian white noise centered at a rescaled version of the previous time variant: 
$$q(x_t|x_{t-1}) = \mathcal{N}(x_t ; \sqrt{\alpha_t} x_{t-1},1-\alpha_t)$$ 
One checks that, if $x_{t-1}$ is Gaussian with variance $\sigma_{t-1}^2$, then so is $x_t$, with variance  $\sigma_t^2 = \alpha_t \sigma_{t-1}^2  +  1-\alpha_t$. Thus unit-variance Gaussian noise is a fixed point of the above process, and the endpoint of the diffusion trajectory. 

### From marginals to SDEs

What is the SDE corresponding to the above diffusion forward trajectory?

## Refereneces 
1. [this blog post](https://yang-song.net/blog/2021/score/) on generative score modeling by Yang Song 
2. 

