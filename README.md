# 2024 Economist/WeThink MRP Estimates

This repository has the constituency-level estimates of our 2024 MRP, conducted with polling from [WeThink](https://wethink.netlify.app/).

# Methodology

To produce these figures, WeThink surveyed a representative sample of 18,595 British adults between May 30th and June 21st. The firm asked respondents which party they planned to support, along with where they lived and basic demographic information about them. Using these data, we built a statistical model—the “multilevel regression” of MRP—to predict the voting intentions for each of 16m possible unique combinations of voters’ age, sex, ethnic group, highest qualification, constituency and voting history. This model is similar to our British “build-a-voter” tool that you can explore here <LINK>. For example, we estimate that a 50 to 54-year-old white woman in Bromsgrove, whose highest qualification is GCSE, who voted to leave the European Union in 2016 and Conservative in 2019, has a 45% chance of voting Conservative again this time and a 29% chance of voting for Reform UK.
The next step, known as “post-stratification”, involves estimating how many people in each of these 16m profiles live in each constituency. In Bromsgrove, there are around 185 people in the group described above, for example, whereas in Bethnal Green and Stepney there are only 5. To produce the final results, we simply multiply the expected vote shares for each party in a given demographic group by the number of people in each constituency who belong to that group.

# Codebook

| Variable    | Description |
| ----------- | ----------- |
| const_cd    | ONS Constituency Code       |
| const_nm    | Constituency Name        |
| winner19    | Notional winner at the 2019 election, from [Rallings and Thrasher](https://interactive.news.sky.com/2024/doc/estimates-2019-general-election-result-new-constituencies-explainer.pdf)        |
| winner23    | Estimated winner      |
| con24    | Estimated Conservative vote share, 2024      |
| green24    | Estimated Green Party vote share, 2024      |
| lab24    | Estimated Labour Party vote share, 2024      |
| ld24    | Estimated Liberal Democrat vote share, 2024      |
| other24    | Estimated "Other" vote share, 2024      |
| pc24    | Estimated Plaid Cymru vote share, 2024      |
| ref24    | Estimated Reform UK vote share, 2024      |
| snp24    | Estimated SNP vote share, 2024      |
| con19    | Notional Conservative vote share, 2019      |
| lab19    | Notional Labour Party vote share, 2019      |
| ld19    | Notional Liberal Democrat vote share, 2019      |
| green19    | Notional Green Party vote share, 2019      |
| snp19    | Notional SNP vote share, 2019      |
| pc19    | Notional Plaid Cymru vote share, 2019      |
| brx19    | Notional Brexit Party vote share, 2019      |
| other19    | Notional "Other" vote share, 2019      |

