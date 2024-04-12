# Design Critique + Redesign

## Part 1: Design Critique  

The radial time series plot below is taken from the following New York Times article:
https://www.nytimes.com/2022/01/06/opinion/omicron-covid-us.html

![image](https://github.com/khushil-sketch/the-Science-of-Data-Visualisations/assets/52947378/7c02c5bb-2805-406b-a637-d91d0963b46b)


The radial chart aims to tell the story of the pandemic's progression (from Jan 2020 to Jan 2022) and the anticipated trajectory of the Omicron variant, underlining the critical moments of increase and decrease in case numbers. By showing past data, it allows for visual comparison with previous waves, and by projecting into the future, it attempts to forecast upcoming trends.
The data displayed is the count of new COVID-19 cases in the United States, captured daily and then aggregated into a 7-day average to smooth out day-to-day fluctuations. The counts are encoded in a red radial line that grows outward from the center, depicting the flow of time. 
The radial line’s area, changes as the number of cases increases, allowing the viewer to see spikes in cases along the outwardly growing line. Time is represented along the circumference, with the months labelled around the edge. This particular visualization captures multiple years of data, allowing for comparison across different phases or waves of the pandemic. At the end of the spiral is the Author’s prediction of what Covid cases will rise to in January 2022 due to the Omicron variant.
I chose this design for critique because it stands out as an unconventional approach to representing time-series data. Traditional linear graphs have been the norm for conveying information about trends over time, and this radial format challenges that standard by introducing a circular depiction of time.

While its aesthetic appeal is undeniable, several issues arise upon critical examination. 
Functionality and Accuracy: One of Albert Cairo's principles is the functionality of a visualization—its ability to accurately depict the data. Here, the radial design introduces complexity that may not enhance the understanding of the data. The radial format makes it challenging to discern the linear trend of COVID-19 cases. Unlike a Cartesian coordinate system, where the x-axis represents time and allows for straightforward comparison of data points across time, the radial format distorts this relationship, particularly as the radial distance from the center increases. This distortion impedes the accurate comparison of case numbers between different months, except at the extremes of high and low values.
Symmetry and Quantitative Precision: The symmetric area around the radial lines can cause confusion. It's unclear whether the area to each side of a central line represents the same data or if the area should be interpreted cumulatively. In a more conventional bar or line graph, the baseline (often at zero) provides a clear reference point from which the magnitude of values can be easily interpreted. Here, the absence of a visible 'zero' line complicates the reading. The precision is compromised by not including specific case count data, which limits the viewer's ability to grasp the exact scale of the pandemic at specific time points.

Labelling and Accessibility: Effective visualization also necessitates that labels and legends are clear and accessible, as they guide the interpretation. The small font size for critical information, such as the indication that the figures are a 7-day average, does not adhere to the best practices of data legibility. A larger, more prominent label would better serve the viewer's understanding.

Scale and Interval Consistency: The design's scale and intervals present additional challenges. As the spiral progresses, the intervals between months widen, which could distort a viewer's perception of the passage of time and the rate of case increases or decreases. Consistent intervals are fundamental for a fair comparison across time periods; hence, the expanding nature of the spiral may inadvertently mislead the viewer.


## Part 2: ReDesign 

Audience: The primary audience for this visualization are public health officials, policymakers, and the general public in the United States. These groups are directly affected by COVID-19 and they care about clear, accurate information regarding COVID-19 to protect their health and the health of their communities.

Big Idea: "Understanding Omicron’s impact on the trajectory of COVID-19 cases 

What is at stake? The public's ability to comprehend and respond appropriately to the evolving COVID-19 situation. The audience needs to understand the progression of the pandemic over time to gauge the current risk level and anticipate future trends. 

Single Person Representation: If this were to be narrowed down to a single person, it would be a local health official who is responsible for communicating risk levels and health guidelines to their community.

Benefits and Risks: If the audience acts on the visualization by following guidelines and supporting policy decisions, the benefits include better health outcomes, fewer COVID-19 cases, and a more controlled environment for managing the pandemic. The risks of inaction or misinterpretation include increased case numbers, higher strain on healthcare systems, and potentially more severe restrictions.
Communication Media: A time series plot will be utilized, given that it is quite suitable for representing data over time
How this plot will address the limitations of the Radial Time Series Plot
Linear Time Representation: To address the difficulty in interpreting trends over time and comparing data points in the radial format, the redesign adopts a linear time series approach. This change ensures that the progression of time is intuitive and that viewers can easily compare the magnitude of case counts across different periods. The linear format preserves the visualization's ability to convey temporal trends while significantly improving readability and interpretability.


Quantitative Precision and Clarity: The critique highlighted the original design's lack of quantitative precision and clear labeling. The redesigned time series plot includes detailed axis labels, a legend explaining any color coding or symbols used, and hover-over tooltips for precise data point information. This approach maintains the original intent to provide detailed data insight while making the information more accessible and understandable.
Consistent and Intuitive Scaling: The radial chart's expanding intervals complicated the comparison of data over time. The redesign uses a consistent linear scale, addressing this limitation. The choice of scale ensures that increments of time and case counts are uniformly represented, facilitating accurate comparisons and preserving the visualization's ability to highlight trends.


Color Usage: While the original visualization's use of color aimed to draw attention, its implementation lacked clarity in conveying information. The redesign uses a color gradient to represent the intensity of COVID-19 cases, with warmer colors indicating higher case counts. This decision not only preserves the original's intent to attract and hold viewer attention but also enhances the chart's informational value by making the data's significance immediately apparent.






