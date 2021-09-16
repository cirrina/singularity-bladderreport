# singularity-bladderreport
Singularity container to use to generate the uroscan bladderreport pdf, html and text using R and knitr. Include R v3.4 and some extras.

This container will only include R, r packeges and other associated libraries that are needed to generate the bladder report.
It will not iclude software for RNAseq analysis.


The main goal is to get include following versions:
r-base=3.4.1 \
r-ranger=0.7.0 \
r-dplyr=0.7.4


Optinally:
r-knitr=1.16
vladsaveliev::r-kableextra=0.9.0
r-jsonlite=1.4

r-reshape=0.8.6
r-ggplot2=2.2.0
r-cowplot=0.9.1



  Also include
  - lynx

  - chromium



  ## v1.0.1
  [percebe@ls4-fe1 rnaseq]$ singularity exec --bind /projects/fs1/ /projects/fs1/shared/ctg-containers/rnaseq/singularity-bladderreport-1.0.1.sif mamba list

                    __    __    __    __
                   /  \  /  \  /  \  /  \
                  /    \/    \/    \/    \
  ███████████████/  /██/  /██/  /██/  /████████████████████████
                /  / \   / \   / \   / \  \____
               /  /   \_/   \_/   \_/   \    o \__,
              / _/                       \_____/  `
              |/
          ███╗   ███╗ █████╗ ███╗   ███╗██████╗  █████╗
          ████╗ ████║██╔══██╗████╗ ████║██╔══██╗██╔══██╗
          ██╔████╔██║███████║██╔████╔██║██████╔╝███████║
          ██║╚██╔╝██║██╔══██║██║╚██╔╝██║██╔══██╗██╔══██║
          ██║ ╚═╝ ██║██║  ██║██║ ╚═╝ ██║██████╔╝██║  ██║
          ╚═╝     ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝╚═════╝ ╚═╝  ╚═╝

          mamba (0.15.3) supported by @QuantStack

          GitHub:  https://github.com/mamba-org/mamba
          Twitter: https://twitter.com/QuantStack

  █████████████████████████████████████████████████████████████

  # packages in environment at /opt/software/uroscan_env:
  #
  # Name                    Version                   Build  Channel
  _libgcc_mutex             0.1                 conda_forge    conda-forge
  _openmp_mutex             4.5                       1_gnu    conda-forge
  _r-mutex                  1.0.1               anacondar_1    conda-forge
  blas                      1.1                    openblas    conda-forge
  bzip2                     1.0.8                h7f98852_4    conda-forge
  ca-certificates           2021.5.30            ha878542_0    conda-forge
  cairo                     1.14.12           ha4e643d_1006    conda-forge
  curl                      7.61.0               h93b3f91_2    conda-forge
  fontconfig                2.13.1            hba837de_1005    conda-forge
  freetype                  2.10.4               h0708190_1    conda-forge
  gettext                   0.19.8.1          hf34092f_1004    conda-forge
  glib                      2.58.3          py37he00f558_1004    conda-forge
  graphite2                 1.3.13            h58526e2_1001    conda-forge
  gsl                       2.2.1           blas_openblashddceaf2_6    conda-forge
  harfbuzz                  1.8.8                hffaf4a1_0
  icu                       58.2              hf484d3e_1000    conda-forge
  jbig                      2.1               h7f98852_2003    conda-forge
  jpeg                      9d                   h36c2ea0_0    conda-forge
  krb5                      1.14.6                        0    conda-forge
  lerc                      2.2.1                h9c3ff4c_0    conda-forge
  libdeflate                1.7                  h7f98852_5    conda-forge
  libffi                    3.2.1             he1b5a44_1007    conda-forge
  libgcc                    7.2.0                h69d50b8_2    conda-forge
  libgcc-ng                 11.1.0               hc902ee8_8    conda-forge
  libgfortran               3.0.0                         1    conda-forge
  libgfortran-ng            7.5.0               h14aa051_19    conda-forge
  libgfortran4              7.5.0               h14aa051_19    conda-forge
  libgomp                   11.1.0               hc902ee8_8    conda-forge
  libiconv                  1.16                 h516909a_0    conda-forge
  libpng                    1.6.37               h21135ba_2    conda-forge
  libssh2                   1.8.0             h1ad7b7a_1003    conda-forge
  libstdcxx-ng              11.1.0               h56837e0_8    conda-forge
  libtiff                   4.3.0                hf544144_1    conda-forge
  libuuid                   2.32.1            h7f98852_1000    conda-forge
  libwebp-base              1.2.1                h7f98852_0    conda-forge
  libxcb                    1.13              h7f98852_1003    conda-forge
  libxml2                   2.9.12               h03d6c58_0
  lz4-c                     1.9.3                h9c3ff4c_1    conda-forge
  ncurses                   6.2                  h58526e2_4    conda-forge
  openblas                  0.3.3             h9ac9557_1001    conda-forge
  openssl                   1.0.2u               h516909a_0    conda-forge
  pandoc                    2.14.2               h7f98852_0    conda-forge
  pango                     1.40.14              he752989_2    conda-forge
  pcre                      8.45                 h9c3ff4c_0    conda-forge
  pip                       21.2.4             pyhd8ed1ab_0    conda-forge
  pixman                    0.34.0            h14c3975_1003    conda-forge
  pthread-stubs             0.4               h36c2ea0_1001    conda-forge
  python                    3.7.1             hd21baee_1001    conda-forge
  python_abi                3.7                     2_cp37m    conda-forge
  r-assertthat              0.2.0            r341h6115d3f_1    conda-forge
  r-backports               1.1.2            r341hc070d10_1    conda-forge
  r-base                    3.4.1                h4fe35fd_8    conda-forge
  r-base64enc               0.1_3            r341hc070d10_2    conda-forge
  r-bh                      1.66.0_1              r341_1001    conda-forge
  r-bindr                   0.1.1            r341h6115d3f_1    conda-forge
  r-bindrcpp                0.2.2            r341h9d2a408_1    conda-forge
  r-callr                   3.0.0            r341h6115d3f_0    conda-forge
  r-cli                     1.0.0            r341h6115d3f_1    conda-forge
  r-clipr                   0.4.1            r341h6115d3f_1    conda-forge
  r-clisymbols              1.2.0            r341h6115d3f_1    conda-forge
  r-colorspace              1.3_2            r341hc070d10_2    conda-forge
  r-cowplot                 0.9.1            r341h3b7045d_0    dranew
  r-crayon                  1.3.4            r341h6115d3f_1    conda-forge
  r-curl                    3.2              r341hc070d10_2    conda-forge
  r-desc                    1.2.0            r341h6115d3f_1    conda-forge
  r-devtools                2.0.1            r341h6115d3f_0    conda-forge
  r-digest                  0.6.18           r341hc070d10_0    conda-forge
  r-dplyr                   0.7.4                  r3.4.1_0    conda-forge
  r-evaluate                0.11             r341h6115d3f_0    conda-forge
  r-fs                      1.2.6            r341h9d2a408_0    conda-forge
  r-ggplot2                 2.2.0                  r3.4.1_0    conda-forge
  r-gh                      1.0.1            r341h6115d3f_1    conda-forge
  r-git2r                   0.23.0           r341h1b3b946_0    conda-forge
  r-glue                    1.3.0            r341h470a237_2    conda-forge
  r-gtable                  0.2.0            r341h6115d3f_1    conda-forge
  r-highr                   0.7              r341h6115d3f_1    conda-forge
  r-hms                     0.4.2            r341h6115d3f_0    conda-forge
  r-htmltools               0.3.6            r341hfc679d8_2    conda-forge
  r-httr                    1.3.1            r341h6115d3f_1    conda-forge
  r-ini                     0.3.1            r341h6115d3f_1    conda-forge
  r-jsonlite                1.4                    r3.4.1_0    conda-forge
  r-kableextra              0.9.0            r341h6115d3f_0    vladsaveliev
  r-knitr                   1.16                   r3.4.1_0    conda-forge
  r-labeling                0.3              r341h6115d3f_1    conda-forge
  r-lazyeval                0.2.1            r341hc070d10_2    conda-forge
  r-magrittr                1.5              r341h6115d3f_1    conda-forge
  r-markdown                0.8              r341hc070d10_3    conda-forge
  r-mass                    7.3_50           r341hc070d10_2    conda-forge
  r-memoise                 1.1.0            r341h6115d3f_1    conda-forge
  r-mime                    0.5              r341hc070d10_2    conda-forge
  r-munsell                 0.5.0            r341h6115d3f_1    conda-forge
  r-openssl                 1.0.2            r341h9f97512_0    conda-forge
  r-pkgbuild                1.0.2            r341h6115d3f_0    conda-forge
  r-pkgconfig               2.0.2            r341h6115d3f_1    conda-forge
  r-pkgload                 1.0.1            r341h9d2a408_0    conda-forge
  r-plogr                   0.2.0            r341h6115d3f_1    conda-forge
  r-plyr                    1.8.4            r341h9d2a408_2    conda-forge
  r-prettyunits             1.0.2            r341h6115d3f_1    conda-forge
  r-processx                3.2.0            r341hc070d10_1    conda-forge
  r-ps                      1.1.0            r341hc070d10_1    conda-forge
  r-r6                      2.2.2            r341h6115d3f_1    conda-forge
  r-ranger                  0.7.0                  r3.4.1_0    conda-forge
  r-rcmdcheck               1.3.0            r341h6115d3f_0    conda-forge
  r-rcolorbrewer            1.1_2            r341h6115d3f_1    conda-forge
  r-rcpp                    1.0.0            r341h9d2a408_0    conda-forge
  r-readr                   1.1.1            r341h9d2a408_2    conda-forge
  r-remotes                 2.0.1            r341h6115d3f_0    conda-forge
  r-reshape                 0.8.6                  r3.4.1_0    conda-forge
  r-reshape2                1.4.3            r341h9d2a408_2    conda-forge
  r-rlang                   0.3.0.1          r341h470a237_0    conda-forge
  r-rmarkdown               1.9                      r341_0    conda-forge
  r-rprojroot               1.3_2            r341h6115d3f_1    conda-forge
  r-rstudioapi              0.7              r341h6115d3f_1    conda-forge
  r-rvest                   0.3.2            r341h6115d3f_1    conda-forge
  r-scales                  1.0.0            r341h9d2a408_1    conda-forge
  r-selectr                 0.4_1            r341h6115d3f_0    conda-forge
  r-sessioninfo             1.1.0            r341h6115d3f_0    conda-forge
  r-stringi                 1.2.4            r341h9d2a408_1    conda-forge
  r-stringr                 1.3.1            r341h6115d3f_1    conda-forge
  r-tibble                  1.3.3                  r3.4.1_0    conda-forge
  r-usethis                 1.4.0            r341h6115d3f_0    conda-forge
  r-viridislite             0.3.0            r341h6115d3f_1    conda-forge
  r-whisker                 0.3_2            r341h6115d3f_1    conda-forge
  r-withr                   2.1.2            r341h6115d3f_0    conda-forge
  r-xml2                    1.2.0            r341h9d2a408_2    conda-forge
  r-xopen                   1.0.0            r341h6115d3f_0    conda-forge
  r-yaml                    2.2.0            r341hc070d10_1    conda-forge
  readline                  7.0               hf8c457e_1001    conda-forge
  setuptools                58.0.4           py37h89c1867_0    conda-forge
  sqlite                    3.28.0               h8b20d00_0    conda-forge
  tk                        8.6.11               h27826a3_1    conda-forge
  wheel                     0.37.0             pyhd8ed1ab_1    conda-forge
  xorg-kbproto              1.0.7             h7f98852_1002    conda-forge
  xorg-libice               1.0.10               h7f98852_0    conda-forge
  xorg-libsm                1.2.3             hd9c2040_1000    conda-forge
  xorg-libx11               1.7.2                h7f98852_0    conda-forge
  xorg-libxau               1.0.9                h7f98852_0    conda-forge
  xorg-libxdmcp             1.1.3                h7f98852_0    conda-forge
  xorg-libxext              1.3.4                h7f98852_1    conda-forge
  xorg-libxrender           0.9.10            h7f98852_1003    conda-forge
  xorg-libxt                1.2.1                h7f98852_2    conda-forge
  xorg-renderproto          0.11.1            h7f98852_1002    conda-forge
  xorg-xextproto            7.3.0             h7f98852_1002    conda-forge
  xorg-xproto               7.0.31            h7f98852_1007    conda-forge
  xz                        5.2.5                h516909a_1    conda-forge
  zlib                      1.2.11            h516909a_1010    conda-forge
  zstd                      1.5.0                ha95c52a_0    conda-forge
