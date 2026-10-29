# Fatal Force: An Investigative Analysis of US Police Shootings

**By Shivansh Yadav**  
*Data Source: The Washington Post Fatal Force Database & US Census Bureau (2015–2017)*

---

## Executive Summary: The 1,000-a-Year Reality

In early 2015, following the deaths of Michael Brown in Ferguson and Eric Garner in New York, it became apparent that the United States government had no reliable, centralized accounting of how many people were fatally shot by police officers each year. *The Washington Post* stepped into that vacuum, launching a nationwide database tracking every on-duty fatal police shooting through public records, local reporting, and community monitoring.

Between January 1, 2015, and July 31, 2017, **2,535 people** were fatally shot by law enforcement in the United States. 

When you dive into the data, the story that emerges isn't just a list of names and incident dates. It is a portrait of structural inequality, mental healthcare deficits, racial disparities, and an unmoving national baseline: roughly **82 Americans die by police gunfire every single month**, or nearly **1,000 people every year**, with no meaningful downward trend across the entire study period.

This report unpacks the humans, the communities, and the systemic patterns behind those numbers.

---

## 1. The Socioeconomic Backdrop: Poverty and Education

Before examining the encounters themselves, we looked at the census data for the communities where Americans live and attend school.

When we compared poverty rates and high school graduation rates across all 50 states, the data revealed an exceptionally strong negative correlation (**$r = -0.806$**):

* **Mississippi** sits at the top of the poverty ranking with an average community poverty rate of **26.88%**, accompanied by one of the lowest graduation rates (**78.5%**).
* **New Jersey** had the lowest average poverty rate (**8.16%**) and one of the highest high school completion rates.
* **Texas** had the lowest average rate of adults over 25 with a high school diploma (**74.09%**), while **Massachusetts** led the country at **92.03%**.

### What This Tells Us
Communities with lower educational attainment and higher poverty face compounding socioeconomic distress. Policing resources, stop-and-frisk tactics, and proactive enforcement are disproportionately deployed in economically depressed neighborhoods, multiplying the frequency of police contacts and, consequently, the likelihood that an encounter escalates to lethal force.

---

## 2. Who is Dying? Demographic Profiles

### The Staggering Gender Disparity
Of the 2,535 victims recorded:
* **Men:** 2,428 (**95.78%**)
* **Women:** 107 (**4.22%**)

That translates to roughly **23 men killed for every 1 woman**. Men are overwhelmingly more likely to be involved in high-threat police encounters, confrontational arrests, and armed standoffs. However, female victims were almost exclusively killed by gunshot alone (99 out of 107), and only 5 women were killed during incidents involving both a firearm and a Taser.

### Age: A Lost Generation
The average age of those killed was **36.6 years old** (median: **35.0 years**). The youngest victim was a 6-year-old child; the oldest was 91.

Nearly **1 in 5 victims (18.31%) was under 25 years old** (450 young lives). 

### The Racial Age Divide: Dying a Decade Younger
When we plotted Kernel Density Estimates (KDE) and analyzed the age curves by race, a critical disparity surfaced:

| Race / Ethnicity | Total Deaths | Share of Known Race | Median Age | Mean Age |
|---|---|---|---|---|
| **White** | 1,201 | 51.32% | **38.0 yrs** | 40.0 yrs |
| **Black** | 618 | 26.41% | **30.0 yrs** | 31.6 yrs |
| **Hispanic** | 423 | 18.08% | **31.0 yrs** | 33.0 yrs |
| **Native American** | 31 | 1.32% | **29.0 yrs** | 30.5 yrs |
| **Asian** | 39 | 1.67% | **35.0 yrs** | 36.6 yrs |
| **Other / Unknown** | 223 | — | 30.0 yrs | 33.1 yrs |

White victims were on average **40 years old**, with a wide, dispersed age distribution extending well into retirement age. 

In sharp contrast, Black, Hispanic, and Native American victims were **systematically and significantly younger**—peaking sharply in their early twenties and early thirties, with median ages of **30, 31, and 29 years old**, respectively. Young men of color are losing their lives nearly a decade earlier than their white counterparts during interactions with law enforcement.

---

## 3. The Circumstances: Weapons, Threat Levels, and Mental Health

### Were People Armed?
One of the most frequent questions in public discourse is whether victims of fatal shootings were armed:
* **Guns:** 1,398 victims (**55.15%**) were armed with a firearm.
* **Knives & Edged Weapons:** 373 victims (**14.71%**).
* **Vehicles:** 177 victims (**6.98%**).
* **Unarmed:** 171 victims (**6.75%**).
* **Toy Weapons:** 104 victims (**4.10%**).
* **Other / Undetermined:** 312 victims.

Overall, **87.6% of individuals were confirmed to be carrying a weapon**, and for every unarmed person killed, more than **8 people armed with guns** were killed. 

Yet, the **171 unarmed deaths** and **104 deaths involving toy guns or replica weapons** represent encounters where the perception of lethal danger by officers resulted in permanent, irreversible loss of life.

### The Mental Health Crisis: When Police Become the Safety Net
Perhaps the most poignant and actionable finding in the entire dataset is this:

> **633 people—or 24.97% (nearly 1 in every 4)—were experiencing an acute mental health crisis or had documented signs of mental illness.**

In many jurisdictions, when a person experiences a psychotic break, suicidal ideation, or severe manic episode, the only first-response service available 24/7 is armed law enforcement. 

Officers trained predominantly in command-and-control tactics and rapid suspect neutralization often arrive at scenes where the individual cannot comprehend or comply with verbal commands. The tragic result is that one-quarter of fatal shootings in America are fundamentally mental healthcare failures rather than conventional law enforcement responses to violent crime.

---

## 4. Geography and Urban Fault Lines

### The Absolute Volume Leaders
By state, the highest raw death counts reflect large overall populations:
1. **California:** 424 deaths
2. **Texas:** 225 deaths
3. **Florida:** 154 deaths
4. **Arizona:** 118 deaths

However, when cross-referenced with poverty rates, states like **Arizona, Oklahoma (78), and Missouri (64)** show an intense convergence of high poverty, loose firearm regulations, and elevated per capita rates of fatal shootings.

### The Top 10 Cities: Stark Racial Overrepresentation
When we examine the top 10 metropolitan areas with the highest number of killings and compare the demographic breakdown of police shootings against the city's racial population share, the disproportions are startling:

```
+---------------+------------------------+--------------------------+-----------------------+
| City          | Total Police Killings  | Black Population Share   | Black Share of Deaths |
+---------------+------------------------+--------------------------+-----------------------+
| Chicago, IL   | 25                     | 32.9%                    | 87.5%  (2.7x)         |
| St. Louis, MO | 15                     | 49.2%                    | 78.6%  (1.6x)         |
| Columbus, OH  | 19                     | 28.0%                    | 61.1%  (2.2x)         |
| Houston, TX   | 27                     | 23.7%                    | 57.7%  (2.4x)         |
| Miami, FL     | 18                     | 19.2%                    | 47.1%  (2.5x)         |
+---------------+------------------------+--------------------------+-----------------------+
```

* **In Chicago**, Black residents make up just under one-third of the city's population, yet **87.5% of individuals shot and killed by police were Black**.
* **In Houston**, Black residents account for **23.7%** of the population but **57.7%** of fatal police shootings.
* **In Columbus**, Black residents make up **28.0%** of the city but **61.1%** of deaths.
* **In Los Angeles and San Antonio**, Hispanic residents constitute the majority of fatalities (**52.8%** in LA, **66.7%** in San Antonio), tracking alongside high rates of police stops in predominantly Latino working-class neighborhoods.

These numbers demonstrate that urban police shootings are not distributed evenly across racial lines or geographic borders; they are concentrated heavily among young men of color living in segregated, historically disinvested neighborhoods.

---

## 5. Time Trends: The Unmoving Needle

We tracked fatal police shootings across all 31 months in the dataset, from January 2015 through July 2017:

* **Monthly Mean:** **81.8 deaths per month**
* **Monthly Minimum:** 65 (June 2015)
* **Monthly Maximum:** 104 (July 2015)
* **Standard Deviation:** 9.33 deaths
* **Linear Trend Slope:** **$-0.038$ deaths/month** (statistically negligible)

```
Monthly Fatal Police Shootings (2015 - 2017)
110 +                                      * (Jul 2015: 104)
100 |                               *             * (Feb 2017: 100)
 90 |             *      *                 *      *
 80 |  *---*----------*------*---*------*------*------*------* (Mean ~82)
 70 |                 *   *             *   *
 60 +
    Jan 15      Jul 15      Jan 16      Jul 16      Jan 17      Jul 17
```

Despite widespread protests, federal investigations, the creation of presidential task forces on 21st-century policing, and intense national media coverage throughout 2015 and 2016, **the national rate of fatal police shootings remained essentially unchanged**. 

Individual departments introduced body cameras and de-escalation training, but on a macro level, American policing continued to take roughly 1,000 lives per year with metronomic regularity.

---

## 6. Synthesis: What the Human Story Demands

Behind each of the 2,535 data points is an individual whose life ended in violence, leaving behind families, communities, and officers forever changed.

The data points to three clear, evidence-based imperatives:

1. **Decouple Mental Health Crisis Response from Armed Policing:**  
   With **1 in 4 victims** suffering from a mental health emergency, dispatching armed officers as primary responders is inherently hazardous. Expanding civilian mobile crisis units (like CAHOOTS in Eugene, Oregon, or STAR in Denver) can resolve psychiatric crises without weapons drawn.

2. **Target Structural Inequities and Urban Disparities:**  
   The extreme overrepresentation of young Black and Hispanic men in urban police shootings is tied directly to concentrated poverty, underfunded schools ($r = -0.81$ correlation with graduation), and neighborhood-based hyper-policing. Lasting reductions in police violence require investing in community stability, youth programs, and economic opportunity.

3. **Institute Mandated, Transparent Federal Reporting:**  
   It should not fall on investigative journalists at *The Washington Post* to maintain the definitive record of state-sanctioned lethal force. Federal reporting must be standardized, audited, and tied to law enforcement grant funding so that policies can be evaluated on real-world outcomes.

---

## Conclusion

The data does not tell a story of a few rogue departments or isolated incidents. Rather, it reveals an interconnected system: poverty concentrates risk, underfunded social services leave police to handle mental illness, systemic racial fault lines dictate who is stopped and scrutinized, and an entrenched operational culture produces a tragically steady toll of 1,000 deaths every year.

Understanding these patterns is the first, necessary step toward changing them.
