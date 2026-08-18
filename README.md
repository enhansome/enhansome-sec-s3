# Awesome sec s3 with stars

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/Amazon-S3-Logo.svg/200px-Amazon-S3-Logo.svg.png" alt="AWS S3" width="120"/>
</p>

<h1 align="center">Awesome AWS S3 Security</h1>

<p align="center">
  <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <a href="https://github.com/mxm0z/awesome-sec-s3/stargazers"><img src="https://img.shields.io/github/stars/mxm0z/awesome-sec-s3?style=flat-square&color=yellow" alt="Stars"></a>
  <a href="https://github.com/mxm0z/awesome-sec-s3/network/members"><img src="https://img.shields.io/github/forks/mxm0z/awesome-sec-s3?style=flat-square" alt="Forks"></a>
  <a href="https://github.com/mxm0z/awesome-sec-s3/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square" alt="License"></a>
</p>

<p align="center">
  <b>A curated collection of tools, techniques, and resources for AWS S3 security research and exposed bucket discovery.</b>
</p>

<p align="center">
  <a href="#bucket-enumeration-tools">Enumeration</a> •
  <a href="#general-purpose-tools">General Purpose</a> •
  <a href="#techniques">Techniques</a> •
  <a href="#articles">Articles</a> •
  <a href="#videos">Videos</a>
</p>

***

## Contents

* [Bucket Enumeration Tools](#bucket-enumeration-tools)
* [General Purpose Tools](#general-purpose-tools)
* [Techniques](#techniques)
* [Articles](#articles)
* [Videos](#videos)
* [Contributing](#contributing)

***

## Bucket Enumeration Tools

> Tools specifically designed for discovering and analyzing AWS S3 buckets

| Tool                                                                                                                          | Description                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| [Grayhat Warfare](http://buckets.grayhatwarfare.com/)                                                                         | Free tool that lists open S3 buckets and helps search for interesting files |
| [AWSBucketDump](https://github.com/jordanpotti/AWSBucketDump) ⭐ 1,473 \| 🐛 8 \| 🌐 Python \| 📅 2024-04-10                   | Quickly enumerate AWS S3 buckets to look for loot                           |
| [S3Scanner](https://github.com/sa7mon/S3Scanner) ⭐ 3,163 \| 🐛 41 \| 🌐 Go \| 📅 2026-08-03                                   | Scan for open AWS S3 buckets and dump the contents                          |
| [s3enum](https://github.com/koenrh/s3enum) ⭐ 278 \| 🐛 2 \| 🌐 Go \| 📅 2026-07-04                                            | Fast Amazon S3 bucket enumeration tool for pentesters                       |
| [s3-buckets-finder](https://github.com/gwen001/s3-buckets-finder) ⭐ 399 \| 🐛 0 \| 🌐 PHP \| 📅 2023-03-28                    | PHP tool to brute force Amazon S3 buckets (by gwen001)                      |
| [s3-buckets-finder](https://github.com/gold1029/s3-buckets-finder) ⭐ 1 \| 🐛 0 \| 🌐 PHP \| 📅 2018-04-27                     | PHP tool to brute force Amazon S3 buckets (by gold1029)                     |
| [Sandcastle](https://github.com/0xSearches/sandcastle) ⭐ 146 \| 🐛 3 \| 🌐 Python \| 📅 2022-12-01                            | Python script for AWS S3 bucket enumeration (formerly bucketCrawler)        |
| [mubrute](https://github.com/GeneralTesler/mubrute)                                                                           | Uses response codes to determine bucket existence and list permissions      |
| [PyLazyS3](https://github.com/Den1al/PyLazyS3) ⭐ 17 \| 🐛 1 \| 🌐 Python \| 📅 2022-01-28                                     | Enumerate AWS S3 buckets using different permutations                       |
| [RoboBucketeer](https://github.com/we45/RoboBucketeer) ⭐ 2 \| 🐛 0 \| 🌐 HTML \| 📅 2018-07-12                                | Robot Framework Library for S3 Buckets & Subdomain Enumeration              |
| [inSp3ctor](https://github.com/brianwarehime/inSp3ctor) ⭐ 126 \| 🐛 1 \| 🌐 Python \| 📅 2021-07-13                           | AWS S3 Bucket/Object Finder                                                 |
| [bucketkicker](https://github.com/craighays/bucketkicker) ⭐ 60 \| 🐛 3 \| 🌐 Python \| 📅 2022-12-08                          | Quickly enumerate AWS S3 buckets and look for loot                          |
| [s3recon](https://github.com/clarketm/s3recon) ⭐ 155 \| 🐛 1 \| 🌐 Python \| 📅 2021-12-27                                    | Amazon S3 bucket finder and crawler                                         |
| [s3finder](https://github.com/magisterquis/s3finder) ⚠️ Archived                                                              | Search using wordlist or certificate transparency logs                      |
| [kicks3](https://github.com/abuvanth/kicks3) ⚠️ Archived                                                                      | S3 bucket finder from HTML/JS and misconfiguration testing tool             |
| [bucket\_finder](https://github.com/mattweidner/bucket_finder) ⭐ 17 \| 🐛 1 \| 🌐 Ruby \| 📅 2016-08-30                       | DigiNinja's bucket\_finder utility                                          |
| [Bucket\_Finder](https://github.com/hazana/Bucket_Finder) ⭐ 0 \| 🐛 0 \| 🌐 Ruby \| 📅 2017-07-20                             | Leaky Buckets finder                                                        |
| [haka\_toni\_bucket\_finder](https://github.com/jjvmak/haka_toni_bucket_finder) ⭐ 1 \| 🐛 0 \| 🌐 JavaScript \| 📅 2019-03-30 | S3 Bucket finder utility                                                    |
| [s3-open-bucket-finder](https://github.com/siddharth2395/s3-open-bucket-finder) ⭐ 0 \| 🐛 0 \| 🌐 Python \| 📅 2019-06-02     | Open S3 Bucket discovery tool                                               |
| [s3scanner](https://github.com/miguelmota/s3scanner) ⚠️ Archived                                                              | Scan for open public S3 buckets                                             |
| [bucket-scraper](https://github.com/Rorkien/bucket-scraper) ⭐ 1 \| 🐛 0 \| 🌐 Java \| 📅 2017-03-23                           | CLI for scraping, indexing and downloading S3 buckets                       |
| [bucket-hunter](https://github.com/samuelcardillo/bucket-hunter) ⭐ 6 \| 🐛 0 \| 🌐 JavaScript \| 📅 2016-01-11                | Amazon AWS Exposed Bucket Hunter                                            |
| [bucket-stream](https://github.com/eth0izzle/bucket-stream) ⭐ 1,808 \| 🐛 9 \| 🌐 Python \| 📅 2025-02-28                     | Find S3 Buckets by watching certificate transparency logs                   |
| [goGetBucket](https://github.com/glen-mac/goGetBucket) ⭐ 116 \| 🐛 0 \| 🌐 Go \| 📅 2019-03-29                                | Penetration testing tool to enumerate S3 Buckets by domain                  |
| [bucket\_finder](https://github.com/FishermansEnemy/bucket_finder) ⭐ 100 \| 🐛 1 \| 🌐 Ruby \| 📅 2013-06-24                  | Trawl Amazon S3 buckets for interesting files                               |

***

## General Purpose Tools

> Multi-purpose tools that include S3 bucket functionality alongside other cloud storage services

| Tool                                                                                                           | Description                                                        |
| -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| [CloudScraper](https://github.com/jordanpotti/CloudScraper) ⭐ 537 \| 🐛 3 \| 🌐 Python \| 📅 2022-03-07        | Enumerate targets for cloud resources (S3, Azure Blobs, DO Spaces) |
| [CloudStorageFinder](https://github.com/digininja/CloudStorageFinder) ⭐ 85 \| 🐛 0 \| 🌐 Ruby \| 📅 2025-10-08 | Find public data in cloud storage systems                          |
| [exif-scraper](https://github.com/downpat/exif-scraper) ⭐ 1 \| 🐛 0 \| 🌐 Python \| 📅 2017-03-22              | Extract EXIF data from S3 bucket photos                            |
| [mlb-dfs-scrapers](https://github.com/kykosic/mlb-dfs-scrapers)                                                | Web scraping for dumping stats to S3 bucket CSV files              |
| [s3m](https://github.com/s3m/s3m) ⭐ 56 \| 🐛 0 \| 🌐 Rust \| 📅 2026-08-16                                     | CLI for streams of data in S3 buckets                              |

***

## Techniques

> Methods and approaches for S3 bucket reconnaissance

### Wayback Machine Enumeration

Use the [enum\_wayback](https://github.com/mubix/stuff/blob/master/metasploit/enum_wayback.rb) ⭐ 32 | 🐛 0 | 🌐 Ruby | 📅 2012-05-25 Metasploit module to pull and parse URLs stored by Archive.org. Useful for finding unlinked and legacy pages during web assessments.

<p align="center">
  <img src="https://i.imgur.com/zSU8dBk.png" alt="enum_wayback demonstration" width="600"/>
</p>

***

## Articles

> In-depth reading about S3 security and misconfigurations

* [List of AWS S3 Leaks](https://github.com/nagwww/s3-leaks) ⭐ 456 | 🐛 0 | 🌐 Python | 📅 2026-08-15 - Comprehensive list of documented S3 data exposures
* [How to Search for Open Amazon S3 Buckets](https://medium.com/@grayhatwarfare/how-to-search-for-open-amazon-s3-buckets-and-their-contents-https-buckets-grayhatwarfare-com-577b7b437e01) - GrayhatWarfare guide
* [There's a Hole in 1,951 Amazon S3 Buckets](https://blog.rapid7.com/2013/03/27/open-s3-buckets/) - Rapid7 research
* [Amazon S3 Bucket Public Access Considerations](https://aws.amazon.com/pt/articles/amazon-s3-bucket-public-access-considerations/) - Official AWS guidance
* [Analysing Amazon's Buckets](https://digi.ninja/blog/analysing_amazons_buckets.php) - DigiNinja analysis
* [Unsecured Public Information in S3 Buckets](https://www.rapid7.com/resources/amazon-s3-bucket-misconfiguration/) - Rapid7 misconfiguration guide
* [Exposed S3 Bucket CloudTrail Logs](https://www.cloudmanagementinsider.com/exposed-s3-bucket-cloudtrail-logs/) - Security implications of exposed logs
* [Fantastic! Public S3 Buckets and How to Find Them](https://auth0.com/blog/fantastic-public-s3-buckets-and-how-to-find-them/) - Auth0 blog

***

## Videos

> Visual learning resources for S3 security

| Title                                                                                                             | Description                                |
| ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| [How do I find out which S3 buckets allow access from the Internet?](https://www.youtube.com/watch?v=xHK_A_lscoA) | AWS guidance on identifying public buckets |
| [Securing and Protecting Against Exposed S3 Buckets](https://youtu.be/UIN-je82K3A)                                | Defensive strategies                       |
| [Effective S3 Bucket Management](https://youtu.be/4tp3pOeKefc)                                                    | Prevention and mitigation techniques       |
| [The Bucket List: Experiences Operating S3 Honeypots](https://youtu.be/k7-wCcS2HFU)                               | Honeypot research insights                 |

***

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

***

<p align="center">
  <sub>If you find this resource helpful, please consider giving it a star!</sub>
</p>

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-18._
