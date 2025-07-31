---
jupytext:
  formats: ipynb,md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: '0.13'
    jupytext_version: 1.14.0
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Welcome to Penghu Atlas Project

>This is a working in progress project website built with Jupyter Book.

The website is served as collaborative hub for documenting materials related to the Penghu Atla project, as well as the info center for depositar API integration. Now, we've tested data on the depositar's [demo site](https://demo.depositar.io/en/). 


// 不知道為什麼以下 folium map code 沒有隱藏 :P
```{code-cell} ipython3
:hide-input:

import folium

# Center the map on Penghu, Taiwan
m = folium.Map(location=[23.565, 119.579], zoom_start=10)
m
```
