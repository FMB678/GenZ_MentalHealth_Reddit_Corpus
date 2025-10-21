# GenZ Mental Health Reddit Corpus

## Overview
This dataset contains a comprehensive collection of mental health discussions from Reddit, specifically focusing on generational differences between GenZ and non-GenZ users. The corpus spans six major mental health subreddits and includes both submissions (original posts) and comments from 2017-2025.

**Dataset**: `GenZ_MentalHealth_Reddit_Corpus/reddit_corpus_sample/`

## Dataset Structure

### File Naming Convention
Files follow the pattern: `{subreddit}_{generation}_{content_type}_sample.xlsx`

- **subreddit**: One of 6 mental health communities
  - `Anxiety`, `depression`, `mentalhealth`, `socialanxiety`, `bipolar`, `bipolar2`
- **generation**: User cohort classification
  - `genz`: Generation Z users
  - `others`: Non-GenZ users
- **content_type**: Type of Reddit content
  - `submission`: Original posts
  - `comment`: Responses to posts

### Data Schema

#### Submission Files (`*_submission_sample.xlsx`)
| Column | Description |
|--------|-------------|
| `author` | Anonymized user identifier |
| `publishing_date` | Post creation date (YYYY-MM-DD) |
| `body` | Text content of the submission |
| `num_comments` | Number of comments on the post |
| `Sentiment` | VADER sentiment score (-1 to +1) |

#### Comment Files (`*_comment_sample.xlsx`)
| Column | Description |
|--------|-------------|
| `author` | Anonymized user identifier |
| `publishing_date` | Comment creation date |
| `body` | Text content of the comment |
| `ups` | Upvotes received |
| `score` | Reddit score metric |
| `Sentiment` | VADER sentiment score (-1 to +1) |

## Corpus Statistics

| Subreddit | GenZ Users | Avg Words | Avg Posts | Submission Words | Avg Submission Words | Comment Words | Avg Comment Words |
|-----------|------------|-----------|-----------|------------------|---------------------|---------------|------------------|
| r/depression | 158,669 | 81.48 | 7.04 | 195,537 | 143.58 | 919,371 | 44.05 |
| r/Anxiety | 84,525 | 73.52 | 8.51 | 82,190 | 154.54 | 634,038 | 47.16 |
| r/mentalhealth | 92,132 | 104.65 | 6.99 | 108,350 | 183.56 | 534,471 | 50.87 |
| r/socialanxiety | 49,741 | 55.94 | 8.06 | 34,061 | 150.49 | 362,309 | 41.12 |
| r/bipolar | 25,239 | 51.81 | 10.26 | 36,006 | 121.55 | 465,362 | 43.89 |
| r/bipolar2 | 7,716 | 58.71 | 23.90 | 9,401 | 152.17 | 173,857 | 49.01 |

## Research Context

### Key Hypotheses Investigated

**H1: GenZ Initiator-Respondent Dynamics**
- GenZ initiators show authentic, negatively-valenced distress expression
- GenZ respondents use positively-valenced support language
- Significant linguistic differences between initiators and respondents across all mental health communities

**H2: COVID-19 Pandemic Impact**
- Pandemic acted as psychological intensifier rather than thematic disruptor
- Significant sentiment declines in depression and anxiety communities during pandemic
- Topic reorganization without structural transformation

**H3: Generational Discourse Differences**
- GenZ discourse: existential, introspective, identity-focused
- Non-GenZ discourse: practical, clinical, management-oriented
- Systematic generational differences in linguistic framing of mental health

### Major Findings
- **Strong initiator-respondent differences** in GenZ communities (p < 0.001)
- **Sentiment declines** most pronounced in depression/anxiety communities during pandemic
- **Generational divide** in mental health conceptualization and expression
- **Platform as developmental niche** for GenZ identity work and social connection

## Usage Notes

### 📁 Files Included
This repository contains sample data files. The complete dataset is available upon request for academic research purposes.

### 🔒 Ethical Considerations
- Contains sensitive mental health discussions
- Intended for academic research only
- Users must comply with ethical guidelines and institutional IRB requirements
