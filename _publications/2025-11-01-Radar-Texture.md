---
title: "Surface Material and Roughness Sensing using mmWave via Surface Scattering and Ambient Vibrations"
collection: publications
permalink: /publication/2025-11-01-Radar-Texture
excerpt: ''
date: 2026-05-11
venue: 'SenSys 2026'
pub_type: 'conference'
authors: 'Yawen Liu, Bert Shan, Swarun Kumar'
paperurl: ''
citation: ''
---

![](/static/image/mmTexora/abstract.png)


Abstract
---
In this paper, we explore a system to sense the roughness of surfaces, even if obstructed from field-of-view. We pose this question in the context of robotic grasping and manipulation to explore if robots can learn the texture of objects prior to grasping them. Importantly, we seek to do so in a completely contact-free fashion (ruling out tactile sensors), despite obstructions (ruling out cameras and lidar). We present mmTexora a novel roughness sensing system using mmWave radar. mmTexora leverages ambient vibrations that produce temporal phase variations to objects in everyday environments, when perceived by radar. We demonstrate how these phase variations convey valuable information about the structure of bumps and ridges on a surface, thereby revealing details about surface roughness. We then develop a signal processing and deep learning pipeline that extracts surface roughness from signal’s temporal variations. mmTexora uses this information to classify surface textures when the material type of an object is known. Conversely, mmTexora can also classify material types for objects when they are known to have similar textures. We perform a qualitative study on a robotic arm tested on diverse objects, where either texture or material type is varied individually. Our classification model achieves an average surface classification accuracy of 93.7% on 50 surfaces that are commonly seen in daily life, with an average absolute error of 0.11 mm in roughness measurements


Recommended citation: 