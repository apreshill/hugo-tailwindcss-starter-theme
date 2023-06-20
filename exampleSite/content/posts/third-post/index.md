---
title: "ggplot2 demo"
author: "Norah Jones"
date: "5/22/2021"
format: 
  hugo-md:
    code-fold: true
    toc: true
---

-   [Air Quality](#air-quality)

## Air Quality

[Figure 1](#fig-airquality) further explores the impact of temperature on ozone level.

<details>
<summary>Code</summary>

``` r
library(ggplot2)

ggplot(airquality, aes(Temp, Ozone)) + 
  geom_point() + 
  geom_smooth(method = "loess"
)
```

</details>

<img src="index.markdown_strict_files/figure-markdown_strict/fig-airquality-1.png" id="fig-airquality" width="768" alt="Figure 1: Temperature and ozone level." />
