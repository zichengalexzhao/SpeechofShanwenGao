# Analysis of Shanwen Gao's Speech

*Alex Zhao | Dec. 2024*

At the end of 2024, [Shanwen Gao](https://www.linkedin.com/in/shanwen-gao-8ab8585/?originalSubdomain=cn) delivered a provocative [speech](https://www.youtube.com/watch?v=1TiZCP5Mnms) that challenged conventional wisdom about China’s economic recovery after the bubble burst. He contended that:

  - **Official GDP figures post-bubble are overstated by roughly 3 percentage points.**
  - **Adjusting GDP downward yields lower predicted consumption growth, closer to what is observed.**
  - **Demographic factors (a higher share of young and elderly populations) further depress consumption growth.**

Intrigued by these claims, I eagerly downloaded data from [National Bureau of Statistics of China](https://www.stats.gov.cn/english/) to put Gao’s assertions to the test. In this project, I lead with the analysis results—my primary focus—as I explore whether his statements hold true and uncover additional insights from his speech:

1. Overstated GDP Figures:
   - The official GDP-to-consumption regression (with an intercept of ~1.81 and slope of ~0.89) predicts much higher consumption growth 
     when applied to official GDP growth figures in the post-bubble period.
   - However, actual observed consumption growth in 2022 was much lower (near -0.25%). When we adjust the GDP growth downward by about 3 percentage points,
     the model predicts consumption growth of ~3.44% (2022) and ~3.27% (2023). This supports Gao Shanwen’s claim that official GDP figures are inflated post-bubble.

2. Structural Break and Protracted Recovery:
   - Gao Shanwen’s speech argues that after the bubble bursts, it takes roughly 9 years for the economy to return to normal growth.
   - The failure of the pre-bubble GDP-consumption relationship (both in the official and adjusted models) to capture the dramatic rebound (e.g., actual consumption growth of 7.22% in 2023) indicates a structural break.
   - This suggests that additional factors are influencing the post-bubble dynamics, consistent with the prolonged adjustment period mentioned in the speech.

3. Demographic Effects:
   - The demographic regression yields the model:
         Consumption Growth = 39.18 + 0.70 * GDP_growth - 119.12 * Young_Share - 139.17 * Elderly_Share
     implying that higher shares of young and elderly populations are associated with significantly lower consumption growth.
   - This finding aligns with the speech’s observation that regions with a higher proportion of young people experience weaker consumption growth,
     likely due to lower income expectations and consumer confidence.
   - The demographic model’s post-bubble predictions (around 1.72% in 2022 and 1.55% in 2023) further underscore the downward pressure on consumption,
     reinforcing the notion of a protracted recovery.

Overall, the empirical results bolster Gao Shanwen’s argument:
   - Official GDP growth figures are likely overstated (by about 3 percentage points).
   - When corrected, the expected consumption growth is significantly lower, reflecting the distorted state of the economy.
   - Demographic pressures further depress consumption, suggesting that a full recovery to pre-bubble levels will take considerable time (on average 9 years).
