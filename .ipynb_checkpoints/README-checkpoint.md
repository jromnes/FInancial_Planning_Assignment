# FInancial_Planning_Assignment

Edits have been made to the 'MCForecastTools.py' file. This was due to the consistent "Performance warning" that I was receiving. I utilized ChatGPT to identify an alternative method that would produce results without the issue of a "Performance Warning".

Lines Edited/Replaced: 117,172 & 173

117(previous): 'portfolio_cumulative_returns[n] = (1 + sim_df.fillna(0)).cumprod()'
117(edited): 'portfolio_cumulative_returns = pd.concat([portfolio_cumulative_returns, (1 + sim_df.fillna(0)).cumprod()], axis=1)'

172(previous): 'return metrics.append(ci_series)'
172&173(edited): 'summary_stats = pd.concat([metrics, ci_series])'
                 'return summary_stats'


