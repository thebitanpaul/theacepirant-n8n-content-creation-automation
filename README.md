# TheAcepirant

> An AI-powered motivational media engine that never stops creating.

<img alt="Hero Image" src="https://res.cloudinary.com/b0tb1mho/image/upload/v1784621250/vf3zn5acvemnopmyjkci.webp"/>

TheAcepirant is a fully automated AI-powered content creation engine that continuously discovers motivational stories, transforms them into engaging narrated short-form videos, and publishes them across **YouTube Shorts, Instagram Reels, and Facebook Reels** with almost no human intervention.

---

## Overview

Creating motivational short-form content consistently requires:

- Discovering inspiring stories
- Writing engaging scripts
- Generating videos
- Publishing across multiple social media platforms
- Managing media assets

Doing this manually is repetitive, time-consuming, and difficult to scale.

TheAcepirant automates the entire workflow—from content discovery to publishing—through an intelligent n8n automation pipeline.

---

## Features

- Reddit Content Discovery
- Smart Content Filtering
- Randomized Story Selection
- AI Script Generation using Google Gemini
- Automated Video Creation
- Rendering Status Monitoring
- Multi-Platform Publishing
- Automatic Retry Logic
- GitHub Temporary Media Hosting
- Automatic Cleanup
- Scheduled Automation Every 4 Hours
- Structured AI Output Parsing


---

## Live Channels

<div align="center">

[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@theacepirant)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/theacepirant)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/profile.php?id=61578929849808)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/thebitanpaul/theacepirant)

</div>


## Gallery

### YouTube Shorts Demo

<a href="https://youtube.com/shorts/Ded5Yg229fc?si=Rk4goaImsZ2qwiJl" target="_blank">
<img src="https://img.youtube.com/vi/Ded5Yg229fc/hqdefault.jpg" width="1080"/>
</a>

### Instagram Reel

<a href="https://www.instagram.com/reel/DNwA6f9xDW0/?igsh=MWJseDdzYnJnNTd3ZQ==" target="_blank">
<img src="https://res.cloudinary.com/b0tb1mho/image/upload/v1784621250/vf3zn5acvemnopmyjkci.webp" width="1080"/>
</a>

### Facebook Reel

<a href="https://www.facebook.com/share/r/1Yw2XKsGja/?mibextid=wwXIfr" target="_blank">
<img src="https://res.cloudinary.com/b0tb1mho/image/upload/v1784621250/vf3zn5acvemnopmyjkci.webp" width="1080"/>
</a>

### Successful Workflow Run

<img alt="Workflow Success" src="https://res.cloudinary.com/b0tb1mho/image/upload/v1784620561/a3gcm1lb0uvmbhgt0qqj.webp"/>

---

## Tech Stack

- n8n
- Google Gemini
- Reddit API
- YouTube Data API
- Instagram Graph API
- Facebook Graph API
- GitHub API
- HTTP API
- MCP
- JSON

---

## Workflow Architecture

```
Schedule Trigger
        │
        ▼
 Reddit API
        │
        ▼
Content Filtering
        │
        ▼
Random Selection
        │
        ▼
 Google Gemini
        │
        ▼
MCP Video Generator
        │
        ▼
Rendering Status Polling
        │
        ▼
Download Generated Video
        │
        ├────────► YouTube Shorts
        │
        ├────────► GitHub Temporary Storage
        │                │
        │                ├────► Instagram Reels
        │                │
        │                └────► Facebook Reels
        │
        ▼
Cleanup Temporary Files
```

---

## Complete Workflow

1. Trigger automatically every four hours.
2. Fetch trending motivational stories from Reddit.
3. Filter low-quality content.
4. Shuffle posts for variety.
5. Generate a motivational narration using Google Gemini.
6. Generate a narrated short-form video.
7. Continuously poll the rendering service until the video is ready.
8. Download the rendered video.
9. Publish to YouTube Shorts.
10. Publish to Instagram Reels.
11. Publish to Facebook Reels.
12. Delete temporary GitHub assets.

---

## Data Flow

```
Schedule Trigger
        │
        ▼
Reddit API
        │
        ▼
Content Filtering
        │
        ▼
Google Gemini
        │
        ▼
MCP Video Generator
        │
        ▼
Rendering Polling
        │
        ▼
Generated Video
        ├────────► YouTube
        ├────────► GitHub
        │              ├────► Instagram
        │              └────► Facebook
        ▼
Cleanup
```

---

## KPIs

| Metric | Value |
|---------|------:|
| Publishing Frequency | Every 4 Hours |
| Video Duration | 10 Seconds |
| Supported Platforms | 3 |
| Success Rate | 95% |
| Manual Effort | ~0 |

---

## Project Metrics

| Metric | Value |
|---------|------:|
| Videos Generated Daily | 6 |
| Publishing Platforms | 3 |
| Automation Level | 100% |
| Source Community | Reddit |

---

## Problem

Producing motivational short-form content consistently requires researching stories, writing scripts, generating videos, publishing to multiple platforms, and managing media assets.

Doing this manually is repetitive, expensive, and difficult to scale.

---

## Solution

TheAcepirant automates the complete content pipeline by:

- Discovering authentic motivational stories
- Generating AI-powered narrations
- Creating narrated short-form videos
- Publishing automatically to multiple platforms
- Cleaning temporary assets after publishing

---

## Architecture

A scheduled n8n workflow orchestrates the entire automation pipeline by retrieving trending Reddit stories, filtering and randomizing content, generating AI narrations with Google Gemini, creating videos through an MCP video generation service, monitoring rendering status, publishing to YouTube Shorts, Instagram Reels, and Facebook Reels, temporarily hosting media on GitHub when required, and finally cleaning temporary assets after successful publishing.

---

## Challenges

- Handling asynchronous rendering
- Waiting for Meta processing
- Managing retries across APIs
- Reliable multi-platform publishing
- Facebook Reel upload requirements
- Temporary asset cleanup

---

## Insights

- AI-generated motivational content enables continuous publishing.
- Polling greatly improves asynchronous reliability.
- Temporary GitHub hosting simplifies Facebook publishing.
- Retry logic improves resilience across APIs.
- Fully automated short-form publishing pipelines scale efficiently.

---

## Key Findings

- Reddit consistently provides authentic motivational stories.
- AI rewriting improves narration quality.
- Every platform has unique publishing requirements.
- Meta requires processing delays before publishing.
- Automatic cleanup keeps storage lightweight.

---

## Outcome

TheAcepirant functions as a fully autonomous AI media engine capable of continuously discovering, generating, and publishing motivational content around the clock with minimal human involvement.

---

## Motivation

Build TheAcepirant into a scalable AI-first motivational media brand capable of continuously producing, publishing, and growing high-quality inspirational content across every major short-form platform.

---

## Status

**Prototype**

---

## Year

2025

---

## License

This project is licensed under the [Apache-2.0](LICENSE).  
See the LICENSE file for full license text.

---

## About phiUture

Welcome to phiUture — Beautiful Technology. Centered Around You. Shaping Tomorrow.

Inspired by the Golden Ratio (φ), our name represents beautiful, intelligent engineering, while the "U" stands for You—placing people at the center of every solution we build.

phiUture is an AI-first software company creating intelligent products, automation systems, and modern digital experiences. This channel documents the journey of building practical AI solutions, from concept to deployment.

```
Here you'll find:
• AI applications and product demos
• AI agents and automation workflows
• Web and mobile app showcases
• Machine Learning and Data Engineering projects
• Product launches and development insights
• UI/UX and software engineering content
• Tutorials, experiments, and future innovations
```

| Personal | Business | Artist |
|----------|----------|--------|
| [![GitHub](https://img.shields.io/badge/GitHub-thebitanpaul-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/thebitanpaul) | [![Website](https://img.shields.io/badge/Website-phiUture-000000?style=for-the-badge&logo=googlechrome&logoColor=white)](https://phiuture.com) | [![YouTube](https://img.shields.io/badge/YouTube-thebitanpaul-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@thebitanpaul) |
| [![LinkedIn](https://img.shields.io/badge/LinkedIn-thebitanpaul-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/thebitanpaul) | [![YouTube](https://img.shields.io/badge/YouTube-phiUture-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@phiuture) | [![Spotify](https://img.shields.io/badge/Spotify-1DB954?style=for-the-badge&logo=spotify&logoColor=white)](https://open.spotify.com/artist/6ghDcCBlKzJIgm3e586jpV) |
| [![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/thebitanpaul) | [![Google Play](https://img.shields.io/badge/Google_Play-Developer-34A853?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/dev?id=6358474525178045834&hl=en) | [![YouTube Music](https://img.shields.io/badge/YouTube_Music-FF0000?style=for-the-badge&logo=youtubemusic&logoColor=white)](https://music.youtube.com/playlist?list=OLAK5uy_km3cjEB2zl59Etcgv9UBKWw800O9G3NdE) |
| [![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://facebook.com/thebitanpaul) | [![Email](https://img.shields.io/badge/Business_Email-thephiuture%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:thephiuture@gmail.com) | [![Amazon Music](https://img.shields.io/badge/Amazon_Music-46C3D0?style=for-the-badge&logo=amazonmusic&logoColor=white)](https://music.amazon.com/albums/B0G52QMYDC) |
| [![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/thebitanpaul_) |  | [![Apple Music](https://img.shields.io/badge/Apple_Music-FA243C?style=for-the-badge&logo=applemusic&logoColor=white)](https://music.apple.com/us/artist/thebitanpaul/1858534880) |
| [![Snapchat](https://img.shields.io/badge/Snapchat-FFFC00?style=for-the-badge&logo=snapchat&logoColor=000000)](https://snapchat.com/t/UgO0Iywr) |  | [![JioSaavn](https://img.shields.io/badge/JioSaavn-2BC5B4?style=for-the-badge&logo=jiosaavn&logoColor=white)](https://www.jiosaavn.com/artist/thebitanpaul-songs/zuo0NgC65gQ_) |
| [![Email](https://img.shields.io/badge/Personal_Email-thebitanpaul%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:thebitanpaul@gmail.com) |  |  |

---

<div align="center">

**2026 · © phiUture · All Rights Reserved**

</div>
