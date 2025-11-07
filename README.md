# Advancing Data in Corrections Example dashboard using Quarto and R

The code in this repository builds an example dashboard using Quarto and R. This is the demo dashboard that was shared during an ADC Academy Office Hours session on November 4, 2025. You can find a link to the video recording of the live demo of building this dashbarod on the [ADC Community Forum](https://forum.advancingdataincorrections.org/t/office-hours-recap-build-a-dashboard-using-quarto/374).

The rendered dashbboard can be viewed here: https://adc-quarto-dash-ex.netlify.app/.

To re-create this dashboard locally, open [`index.qmd`](https://github.com/CSGJusticeCenter/adc_quarto_dash_ex/blob/main/index.qmd) and render to HTML. The needed data is contained in the [`data/`](https://github.com/CSGJusticeCenter/adc_quarto_dash_ex/tree/main/data) folder. See below for installed package versions.


```
─ Session info ─────────────────────────────────────────────────────────────────────────────────────────────────
 setting  value
 version  R version 4.4.2 (2024-10-31 ucrt)
 os       Windows 11 x64 (build 26200)
 system   x86_64, mingw32
 ui       RStudio
 language (EN)
 collate  English_United States.utf8
 ctype    English_United States.utf8
 tz       America/New_York
 date     2025-11-07
 rstudio  2025.09.1+401 Cucumberleaf Sunflower (desktop)
 pandoc   3.6.3 @ C:\\Users\\mherman\\AppData\\Local\\Programs\\Quarto\\bin\\tools\\pandoc.exe

─ Packages ─────────────────────────────────────────────────────────────────────────────────────────────────────
 package     * version date (UTC) lib source
 askpass       1.2.1   2024-10-04 [1] CRAN (R 4.4.2)
 cli           3.6.3   2024-06-21 [1] CRAN (R 4.4.2)
 credentials   2.0.2   2024-10-04 [1] CRAN (R 4.4.2)
 curl          6.0.1   2024-11-14 [1] CRAN (R 4.4.2)
 evaluate      1.0.1   2024-10-10 [1] CRAN (R 4.4.2)
 fansi         1.0.6   2023-12-08 [1] CRAN (R 4.4.2)
 fs            1.6.5   2024-10-30 [1] CRAN (R 4.4.2)
 gert          2.1.4   2024-10-14 [1] CRAN (R 4.4.2)
 gh            1.4.1   2024-03-28 [1] CRAN (R 4.4.2)
 gitcreds      0.1.2   2022-09-08 [1] CRAN (R 4.4.2)
 glue          1.8.0   2024-09-30 [1] CRAN (R 4.4.2)
 httr2         1.0.7   2024-11-26 [1] CRAN (R 4.4.2)
 jsonlite      1.8.9   2024-09-20 [1] CRAN (R 4.4.2)
 knitr         1.49    2024-11-08 [1] CRAN (R 4.4.2)
 lifecycle     1.0.4   2023-11-07 [1] CRAN (R 4.4.2)
 magrittr      2.0.3   2022-03-30 [1] CRAN (R 4.4.2)
 openssl       2.2.2   2024-09-20 [1] CRAN (R 4.4.2)
 pillar        1.9.0   2023-03-22 [1] CRAN (R 4.4.2)
 pkgconfig     2.0.3   2019-09-22 [1] CRAN (R 4.4.2)
 purrr         1.0.2   2023-08-10 [1] CRAN (R 4.4.2)
 R6            2.5.1   2021-08-19 [1] CRAN (R 4.4.2)
 rappdirs      0.3.3   2021-01-31 [1] CRAN (R 4.4.2)
 rlang         1.1.4   2024-06-04 [1] CRAN (R 4.4.2)
 rprojroot     2.0.4   2023-11-05 [1] CRAN (R 4.4.2)
 rstudioapi    0.17.1  2024-10-22 [1] CRAN (R 4.4.2)
 sessioninfo   1.2.2   2021-12-06 [1] CRAN (R 4.4.2)
 sys           3.4.3   2024-10-04 [1] CRAN (R 4.4.2)
 tibble        3.2.1   2023-03-20 [1] CRAN (R 4.4.2)
 usethis       3.1.0   2024-11-26 [1] CRAN (R 4.4.2)
 utf8          1.2.4   2023-10-22 [1] CRAN (R 4.4.2)
 vctrs         0.6.5   2023-12-01 [1] CRAN (R 4.4.2)
 withr         3.0.2   2024-10-28 [1] CRAN (R 4.4.2)
 xfun          0.49    2024-10-31 [1] CRAN (R 4.4.2)

 [1] C:/Users/mherman/AppData/Local/R/win-library/4.4
 [2] C:/Program Files/R/R-4.4.2/library

```
