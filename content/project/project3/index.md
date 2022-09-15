---
title: Tidal Heating of Exomoons and Detection Methods
summary: Moons in resonance can be significantly heated, and this has implications for exomoon detection.
tags:
  - Project 3
# date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by NASA/JPL/Space Science Institute
  focal_point: Smart

links:
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Jupiter's moons provide valuable sources of information that can be applied to exomoons around exoplanets. For example, Io and Europa are in a 2:1 resonance, meaning Europa's orbital period is twice that of Io (3.50 days vs 1.75 days), and Io is significantly tidally heated. Motivated by this interesting configuration, we studied how two exomoons in resonance would be tidally heated. Without being in resonance, an exomoon is likely to be in a circular orbit due to tides, and there would be no tidal heating. Thus, between two moons, we focus on the inner one whose orbit is constantly being perturbed by the outer moon. By converting physical parameters like semi-major axis and eccentricity into canonical coordinates x and y, we map this perturbation, or libration, as a simple curve. The plots below are examples. The left plot is for arbitrary values and the moon experiences significant libration: there is a large curve around the red dots, or fixed points, where there would be minimum perturbation. The plot on the right is for Jupiter-Io-Europa and the small circle around the fixed point makes it clear that this system experiences far less libration. In other words, it's close to perfect resonance.

<img style="padding-left: 10px; padding-bottom: 0px; padding-top: 0px" src="./contours.png" width="800px" height="600px">

To track this perturbation and resulting tidal heating, we used the N-body numerical integrator code [REBOUND](https://rebound.readthedocs.io/en/latest/) to simulate theoretical systems made up of two exomoons in resonance around an exoplanet. The inner moon starts off on a circular orbit, with zero tidal heating, but simulations show that the eccentricity is quickly pumped up, leading to an overall significantly heated moon. The plots to the right show results for moons in 2-4 day orbits and 4-8 day orbits around Earth-like and Neptune-like planets. The moon in a two day orbit around an Earth-sized planet experiences the most heating: up to 481 K!

<img style="float: right; padding-left: 10px; padding-bottom: 0px; padding-top: 0px" src="./heating.PNG" width="400px" height="500px">

<!---
 <img id="myimage" style="padding-left: 10px; padding-bottom: 0px; padding-top: 0px" src="./transit.gif" width="500px" height="500px">
--->
<img src="./transitstill2.PNG" onmouseover="this.src='./transit.gif'" onmouseout="this.src='./transitstill2.PNG'" />
