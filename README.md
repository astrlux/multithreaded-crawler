# Multithreaded Web Crawler
This Spider Program fetches all of the hyperlinks on a webpage, storing them in a ".txt" file on your system. Some of my personal projects need this type of information so I created this web crawler with the help of an online [tutorial](https://www.youtube.com/playlist?list=PL6gx4Cwl9DGA8Vys-f48mAH9OKSUyav0q). The links can also be returned in a ".csv" format with minor adjustments to *general*.py, lines 13 & 14. 

> In addition to the runtime benefits from multithreading, this program doesn't explore external links which could taint your data set. In other words, this program stays under the umbrella of the domain and doesn't wander off of your specified website. If you so desire, this feature can be toggled easily, however.   

### Overview
This web crawler uses multithreading processes to increase the crawl rate. By default, it runs 8 different threads (or 8 horitzonally isolated "spiders"). The thread count *should be adjusted* depending on the computing power and the unique nature of your webpage. Every single thread shares the same harvesting queue and progress is updated in real-time which prevents overlap.
    
### Basic User Instructions
 1. Import this project into a Python IDE (after cloning this repo onto your local machine).
 2. Manually enter the url of the webpage you want to crawl into *main*.py (line 8).
 3. Run *main*.py –– you can monitor the crawl progress by looking at the console output of your IDE (depending on the nature of your website, the program may take seconds/hours/days to finish running).
 4. When the program is finished running, all of the hyperlinks can be access in *crawler.txt* (which is stored in the same directory as this project).


 ![alt text][spider]
 
[spider]: https://images-platform.99static.com/HBjSN7zLjJvJHqiWlGS940ySqew=/500x500/top/smart/99designs-contests-attachments/55/55065/attachment_55065923

By Uposhanto Bhattacharya, 2019.
