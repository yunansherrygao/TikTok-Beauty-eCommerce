We combined two complementary data sources: TikTok's Research API (3,184 beauty
videos with engagement metrics and creator profile data) and Fastmoss, a third-party TikTok
analytics platform (2,664 ad videos with ROAS and ad spend, plus 2,222 brand-level records).
Because neither dataset alone could answer our research questions. TikTok API lacks ad
performance data while Fastmoss lacks creator follower information (such as their follower
amount, which is an important metric we use to divide creators into different tiers). We merged
the two on creator username and video ID, enabling cross-dataset analyses such as linking
creator tier to ROAS.
Our methods were chosen to match each question's structure. For the market-level
analysis, we used multiple linear regression to test content features as ROAS predictors, TF-IDF
with K-Means clustering and ANOVA to examine hashtag theme effects on engagement and
ROAS, K-Means clustering on brand-level metrics to identify strategy archetypes, and linear
regression to assess ad duration's effect on revenue across brand clusters.
For the Medicube case study, we employed Propensity Score Matching (PSM) to
estimate the causal effect of video boosting on sales — deliberately excluding view count as a
matching covariate since it lies on the causal pathway (Boost → Views → Sales). We validated
this through three model specifications and confirmed robustness via Standardized Mean
Difference diagnostics. We also ran log-log OLS regression with HC3 robust standard errors on
6,000 videos, ANOVA with Tukey HSD post-hoc tests on creator tier GPM (gross merchandise
per 1,000 views), and rank-based methods (Spearman correlation, Kruskal-Wallis) for the 32-
product portfolio analysis where the small sample size precluded parametric approaches.
