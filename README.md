# ITA-ELECTION-2022: A multi-platform dataset of social media conversations around the 2022 Italian general election
This is a repository of social media posts related to the Italian 2022 general election. For more details about the collection procedure see the related dataset paper:

<b> ITA-ELECTION-2022: A multi-platform dataset of social media conversations around the 2022 Italian general election" Pierri Francesco, Liu Geng, Ceri Stefano (2023) </b> <br> 

If you use this data please don't forget to cite the paper, thanks!

## Files description

`fb_ids_urls` and `ig_ids_urls` contain daily ".csv" files for Facebook and Instagram data, respectively. Rows provide the <i>platformId</i> and <i>postUrl</i> of each post, which can be used to retrieve the original post via Crowdtangle or access it in the browser directly (for more details see [Crowdtangle]([https://github.iu.edu/NaN-team/midterm2022/wiki](https://github.com/CrowdTangle/API/wiki)) documentation) <br>

`tw_ids` contains daily ".txt" files for Twitter data. Each file provides IDs of tweets that can be used to re-hydrate tweets using [Hydrator](https://github.com/DocNow/hydrator) or [Twarc](https://github.com/DocNow/twarc). <br>

`keywords.txt` contains the list of election-related keywords employed for collecting the data on different platforms. These were obtained through a snowball sampling approach starting with seeds such as "elezioni" or "elezioni2022". <br>

`meta_ads_ids.txt` contains the list of IDs of ads collected in the dataset. These can be used to retrieve ads through [Meta Ad Library](https://www.facebook.com/ads/library) API or search console. <br>

`*_metadata.csv` files contain metadata for YouTube and TikTok videos shared on Twitter and Facebook. YouTube metadata was collected through the official API whereas TikTok metadata was scraped using [pyktok](https://github.com/dfreelon/pyktok) library <br>

`*_representative_handles.csv` files contain social media handles associated to Italian representatives. <br>


## Acknowledgments
We are thankful to M.Sc. students Valeria Panté and Ilaria Saini for helping match social media accounts to political representatives. Work supported in part by PRIN grant HOPE (FP6, Italian Ministry of Education).
