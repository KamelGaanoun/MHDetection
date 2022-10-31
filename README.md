# Mawdu Hadith Detection

# What is the repository is about?
This is the repository accompanying our paper [Fabricated Hadith Detection: A Novel Matn-Based Approach with Transformer Language Models](https://ieeexplore.ieee.org/abstract/document/9931123). In the paper, we introduce:

- A Matn-based Mawdu (Fabricated) Hadith (MH) detection system
- Two new datasets, called NAH Plus and MAHADDAT
- A comprehensive comparison study between numerous
classical ML algorithms and Arabic TLMs in Hadith
authentication performance.

This repository describes the datasets creation process and gives their content details.


## Table of Contents
- [Description](#description)
- [Dataset](#dataset)
- [Citation](#citation)
- [License](#license)

## Description

Our final dataset relies on [LK](https://github.com/ShathaTm/LK-Hadith-Corpus) and [NAH](https://github.com/TaghreedT/NAH-Corpus) corpora. We adopt a 3-step process as described in the figure below. **NAH Plus** is an enhanced version of NAH corpus, obtained after cleaning and scrapping steps. This corpus contains a total of 3,660 non-authentic Hadiths. We filter the NAH Plus dataset to extract the MHs, and the same process was applied to the LK corpus, which contains 29 MHs. In addition, we add the 366 MHs scraped from [Dorar](https://Dorar.net) and delete any duplicates. As a result, we create a new corpus dedicated to MHs, with a total of 2,452 Hadiths. We call this dataset **MA**wdu **HAD**ith **DAT**aset or **MAHADDAT**.

<p align="center">
  <img src=GA.jpg />
</p>


The following table summarizes some statistics on the final dataset.


<table class="tg">
<thead>
  <tr>
    <th class="tg-fymr" colspan="2" rowspan="2">Number of Hadiths</th>
    <th class="tg-fymr" colspan="3">Number of characters</th>
    <th class="tg-fymr" colspan="3">Number of words</th>
  </tr>
  <tr>
    <th class="tg-fymr">Including diacritics</th>
    <th class="tg-fymr">Excluding diacritics</th>
    <th class="tg-fymr">Excluding diacritics<br>and punctuation</th>
    <th class="tg-fymr">Total</th>
    <th class="tg-fymr">Avg.</th>
    <th class="tg-fymr">Max.</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-fymr">Sahih</td>
    <td class="tg-0lax">24,109</td>
    <td class="tg-0pky">7,937,516</td>
    <td class="tg-0pky">5,025,378</td>
    <td class="tg-0pky">4,969,969</td>
    <td class="tg-0pky">1,016,116</td>
    <td class="tg-0pky">~42</td>
    <td class="tg-0pky">1,698</td>
  </tr>
  <tr>
    <td class="tg-fymr">Mawdu</td>
    <td class="tg-0lax">2,452</td>
    <td class="tg-0pky">576,345</td>
    <td class="tg-0pky">542,933</td>
    <td class="tg-0pky">528,824</td>
    <td class="tg-0pky">109,836</td>
    <td class="tg-0pky">~45</td>
    <td class="tg-0pky">5,608</td>
  </tr>
  <tr>
    <td class="tg-fymr">Total</td>
    <td class="tg-0lax">26,561</td>
    <td class="tg-0pky">8,513,862</td>
    <td class="tg-0pky">5,568,312</td>
    <td class="tg-0pky">5,498,794</td>
    <td class="tg-0pky">1,125,952</td>
    <td class="tg-0pky">~42</td>
    <td class="tg-0pky">5,608</td>
  </tr>
</tbody>
</table>





You may refer to our paper, cited below, for more details on this process.

## Dataset

The final dataset is split into Train/Dev/Test subsets using a 80/10/10 split strategy. These partitions along with NAH Plus and Mahaddat are available for direct donwload in the appropriate folders of this repository.
                      
## Citation

Please cite the following paper if you decide to use the dataset:

    Gaanoun, Kamel, and Mohammed Alsuhaibani. "Fabricated Hadith Detection: A Novel Matn-Based Approach with Transformer Language Models." IEEE Access (2022).
    
## License
The datasets are distributed under the CC BY 4.0 license.
