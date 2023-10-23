# ITA-ELECTION-2022: A multi-platform dataset of social media conversations around the 2022 Italian general election
This is a repository of social media posts related to the Italian 2022 general election. For more details about the collection procedure see the related dataset paper:

<b> Francesco Pierri, Geng Liu, and Stefano Ceri. 2023. ITA-ELECTION-2022: A Multi-Platform Dataset of Social Media Conversations Around the 2022 Italian General Election. In Proceedings of the 32nd ACM International Conference on Information and Knowledge Management (CIKM '23). Association for Computing Machinery, New York, NY, USA, 5386–5390. https://doi.org/10.1145/3583780.3615121 </b> <br> 

```
@inproceedings{10.1145/3583780.3615121, author = {Pierri, Francesco and Liu, Geng and Ceri, Stefano}, title = {ITA-ELECTION-2022: A Multi-Platform Dataset of Social Media Conversations Around the 2022 Italian General Election}, year = {2023}, isbn = {9798400701245}, publisher = {Association for Computing Machinery}, address = {New York, NY, USA}, url = {https://doi.org/10.1145/3583780.3615121}, doi = {10.1145/3583780.3615121}, abstract = {Online social media play a major role in shaping public discourse and opinion, especially during political events. We present the first public multi-platform dataset of Italian-language political conversations, focused on the 2022 Italian general election taking place on September 25th. Leveraging public APIs and a keyword-based search, we collected millions of posts published by users, pages and groups on Facebook, Instagram and Twitter, along with metadata of TikTok and YouTube videos shared on these platforms, over a period of four months. We augmented the dataset with a collection of political ads sponsored on Meta platforms, and a list of social media handles associated with political representatives. Our data resource will allow researchers and academics to further our understanding of the role of social media in the democratic process.}, booktitle = {Proceedings of the 32nd ACM International Conference on Information and Knowledge Management}, pages = {5386–5390}, numpages = {5}, keywords = {multi-platform, italy, social media, politics, advertisement}, location = {Birmingham, United Kingdom}, series = {CIKM '23} }
```

If you use this data please don't forget to cite the paper above, thanks! <br>

Contact: francesco.pierri at polimi.it

## Files description

`fb_ids_urls` and `ig_ids_urls` contain daily ".csv" files for Facebook and Instagram data, respectively. Rows provide the <i>platformId</i> and <i>postUrl</i> of each post, which can be used to retrieve the original post via Crowdtangle or access it in the browser directly (for more details see [Crowdtangle]([https://github.iu.edu/NaN-team/midterm2022/wiki](https://github.com/CrowdTangle/API/wiki)) documentation) <br>

`tw_ids` contains daily ".txt" files for Twitter data. Each file provides IDs of tweets that can be used to re-hydrate tweets using [Hydrator](https://github.com/DocNow/hydrator) or [Twarc](https://github.com/DocNow/twarc). <br>

`keywords.txt` contains the list of election-related keywords employed for collecting the data on different platforms. These were obtained through a snowball sampling approach starting with seeds such as "elezioni" or "elezioni2022". <br>

`meta_ads_ids.txt` contains the list of IDs of ads collected in the dataset. These can be used to retrieve ads through [Meta Ad Library](https://www.facebook.com/ads/library) API or search console. A repository containing screenshots of these ads is available [here](https://github.com/ruggsea/2022IT-election-ads) <br>

`*_metadata.csv` files contain metadata for YouTube and TikTok videos shared on Twitter and Facebook. YouTube metadata was collected through the official API whereas TikTok metadata was scraped using [pyktok](https://github.com/dfreelon/pyktok) library <br>

`*_representative_handles.csv` files contain social media handles associated to Italian representatives. <br>


## Twitter data ##
Given future limitations that will be likely introduced to public APIs, we encourage interested researchers to reaching out to us in case they find difficulties in accessing Twitter data.

## Acknowledgments
We are thankful to M.Sc. students Valeria Panté and Ilaria Saini for helping match social media accounts to political representatives. Work supported in part by PRIN grant HOPE (FP6, Italian Ministry of Education).
