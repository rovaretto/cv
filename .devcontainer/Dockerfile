FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

ENV DEBIAN_FRONTEND=noninteractive

# TeX Live packages needed to compile this CV (Source Sans Pro, Font Awesome 5, etc.)
RUN apt-get update \
  && apt-get install -y --no-install-recommends \
    latexmk \
    texlive-latex-base \
    texlive-latex-recommended \
    texlive-latex-extra \
    texlive-fonts-recommended \
    texlive-fonts-extra \
    texlive-lang-english \
    texlive-pictures \
    lmodern \
  && rm -rf /var/lib/apt/lists/*

WORKDIR /workspaces/cv
