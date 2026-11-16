# <picture><img src="https://ga-curriculum.github.io/universal-resources-internal/ga-logos/ga-red-cog-128x128.png" alt="" height="48" align="absmiddle"></picture> Presentation Advice

How do you give a technical presentation to a nontechnical audience? What about to a technical audience? Below I give advice based on years of experience giving presentations both as a data scientist and data science instructor.

## General Presentation Advice (regardless of audience)
- **Don't show heatmaps, ever.**
    * Why? They're large and overwhelming. Presentation slides should contain as much information as possible with as little brainpower as possible. Heatmaps are antithetical to this.
    * Heatmaps are great viz for you, the data scientist. They're _exploratory_, not _explanatory_.
- **Don't use green and red together.** Red-green colorblindness is much more common than you think. An optimal substitute is to use blue and orange.
- **Don't use monospace fonts.** Code-style fonts are called "monospace" because every character is the same width. Never use it in a presentation. To a nontechnical audience, this makes them feel like they're looking at computer code and they will think what they're seeing is more complicated than it is. To a technical audience, it just makes your presentation look unfinished. This mostly means you'll need to ensure all of your graph labels are custom-made.
- **Graphs should be high-res.** Blurry graphs just look unprofessional. You can increase your graph's resolution by using `plt.savefig(... dpi=192)`.
- **Graphs should not use default colors.** The default Matplotlib blue is hideous and we all know exactly what it looks like. Using this color makes your graph look rushed. Just make it pretty! I generally use `"navy"` as a quick professional-looking graph color.

## Advice for Presenting to Nontechnical Audiences
- **Be mindful of what a nontechnical person actually knows.** You might begin DSI as a nontechnical person, and as you learn more in our class, might come to believe that all nontechnical people know what a correlation coefficient is. Try to remember what it was like before DSI!
- **Explain technical terms you use, but keep the explanations nontechnical.** This is the hard bit. 
    * Example 1, Correlation: "The correlation between two numeric variables describes how tight their relationship is. Numbers close to 1 imply a strong positive relationship, close to -1 implies a strong negative relationship, and close to 0 implies no relationship."
    * Example 2, Decision trees: "A decision tree is a statistical model that uses yes/no questions to make predictions. For example, are you above the age of 30? Do you make more than $60,000 per year? If so, then you're likely to buy our product."
- **Avoid presenting numbers have no human-interpretable explanation, if possible.** The MSE is meaningless to a human. When comparing multiple ML models, try not to use it at all in favor of something more human-interpretable like R2 or MAE. If you really must present MSE, accompany it with a nontechnical explanation, for example "This number represents the quality of model fit. It's not interpretable to us, but lower is better."

## Advice for Presenting to Technical Audiences
- **You still need to explain things!** Just because your audience is technical doesn't mean they know everything. You'll still need to explain what an SVM is. Very few people can immediately recall the difference between precision and recall. The key difference is that your explanations are allowed to be technical. Feel free to use equations.
- **DS is still not really standardized - you still need to be specific.** Is the denominator of MSE _n_ or _n - p_? The term "panel data" can literally mean the opposite thing to different audiences. Does that matrix include the intercept column or not? Is that a rate or shape parameter in your exponential distribution? Be specific!
- **Don't get lost in the weeds.** There's no such thing as a presentation that is only technical. Don't forget to explain the basics of the subject matter to your audience! Don't lose sight of the subject for the technicals.
