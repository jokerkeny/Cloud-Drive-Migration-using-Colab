<!--
 * @Author: jokerkeny
 * @Date: 2021-02-10 16:13:12
 * @LastEditors: jokerkeny
 * @LastEditTime: 2021-02-10 20:23:01
 * @Description: file content
-->
# Cloud Drive Migration using Colab
Migration of files from Baidu Yun to Google Drive.

which is fast, and doesn't occupy your local bandwidth.

## About
Most ISPs provide quite low, such as 1M, 10M upload bandwidth, compared to 100M, 300M download bandwidth, so even if you've downloaded files from baidu yun using paid SVIP to accelerate, it's painful to upload it to Google Drive.  

However, it's fast to transfer file from Google cloud service to Google Drive.  

While GCE(Google Cloud's Compute Engine) is paid service, Google Colab is FREE! and colab is much easier to set up.  

This solution use Google Colab to migrate your files from Baidu Yun to Google Drive, with the help of a Baidu Yun Python Client [bypy](https://github.com/houtianze/bypy). 

## Usage
Use colab to open migration.ipynb(you can do it just by clicking https://colab.research.google.com/github/jokerkeny/Cloud-Drive-Migration-using-Colab/blob/main/migration.ipynb). **Remember use the Google account with Google Drive you want to store**

Follow the instructions in the notebook.

## Speed limit
*The following number is according to my own testing result of this script, including the VIP boosting part*

Baidu yun has a download speed limit of 78Kb/s, You could buy some speed booster from baidu (SVIP, day card, or idle time booster, since the drive migration work could be done in several days), normally it would boost the speed to 4 Mb/s(single file on 4Mb/s, multiple files with multiple processes can be fast as 7Mb/s in total)

The network from Colab to Google Drive usually won't be the bottleneck.

## Acknowledge
This project can't exist without bypy (https://github.com/houtianze/bypy)
