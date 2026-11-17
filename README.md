# Anecdotal-LLM

## Motivation ##
The motivation for the project stems from the lack of available data for researchers studying illicit markets. Building from the concept of mosaic theory, by linking separate, seemingly immaterial pieces of information, one can create a larger and more valuable picture. 

The project listed here is specifically focused on identifying cities connected through the cocaine trade in Europe. While this scope is limited, I believe the steps here are generalizable for developing "anecdotal" evidence by scrapping a wide range of sources. 

I make no claims on being an expert at using LLMs for research, but I believe the below process is a fairly intuitive step-by-step guide to what I use. I will be as clear as possible about the steps and my motivation for proceeding this way. This is meant as an open source tool for other researchers so please take this an improve on the process. If you find steps that can be improved please let me know. 

Eligible documents to be used in the process include anything discussing official events in the drug trade. Most often researchers rely on data from international organizations such as the UNODC or Europol, which aggregate information and release documents to the public highlighting this information. However the connections are not always as detailed as one would hope, and the source material is often not sharable with researchers. In order to develop original, publicly available source material I cast a wider net by allowing the same official documents from international organizations, but also allowing news reports, blog posts, press releases, and other document types. 

## Programs used
1. RStudio
2. BraveSearch API
3. Ollama
4. qwen2.5vl:3B

## Steps
1. develop prompts for BraveSearch API. This will identify what sort of keyword combinations should be used. I used prompt augmentation to create the prompts.
2. run BraveSearch prompt in R.(you will need a BraveSearch API key. You can create an account for free and receive $5 free in calls.)
3. manually spot check urls from BraveSearch and deduplicate
4. develop prompt using prompt augmentation. Be clear to specify which model you are using for the LLM scrape.
5. run LLM scrape in R



