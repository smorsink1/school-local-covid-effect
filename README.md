# University Reopenings and Local COVID Severity
Quantifying the effect of university reopenings on COVID severity in surrounding area

## The Question

What effect did university reopenings have on COVID cases and deaths in their surrounding communities?

## The Data

From the New York Times, there is time-series data on county-level COVID cases and deaths.

From US News and World Report, there is data on university characteristics.

From the College Crisis Initiative at Davidson College, there is data on university reopening policies.

From the New York Times, there is data on total cases at universities since the beginning of the pandemic. 

## The Methdology

There is pseudo-random variation on two fronts: whether a county has schools or not, and school reopening policies. By comparing local COVID situations in otherwise similar counties, some with schools and some without schools, or by comparing local COVID situations in otherwise similar counties, some with in-person instruction schools and some with online instruction schools, we can hope to identify the causal effect of school reopening policies.

## The Challenges

The treatment (a school's reopening policy) is at the school level, while the outcome (a county's COVID cases and deaths) is at the county level. A potential workaround is focusing on counties where virtually all of the students are at one school, or by somehow aggregating the various schools in a county's policies into a single description of school policy in that county.

More generally, great care must be taken when defining the treatment variable.

It is unclear whether or not cases at schools are included in county's case numbers. A potential workaround is focusing on deaths, under the assumption that a low number of deaths occur among those at universities, and therefore the differences between including and not including school deaths in county numbers is small.

A confounding variable is the policies of the county. Suppose there are otherwise similar counties, one with "lax" county COVID policies and one with "strict" county COVID policies. Schools in the "strict" counties will be more likely to have online reopenings, and also have more likely to have lower COVID transmission due solely to the county policy. Schools in the "lax" counties will be more likely to have in-person reopenings, and also more likely to have higher COVID transmission. Therefore, without accounting for county policies (which we don't have data on as of now), we risk overestimate the causal effect of school reopenings (an online reopening be associated with lower transmission solely because of county rules, not because of the reopening itself). 

## Sources of Heterogeneity in Treatment Effect

Some have pointed out that school reopening policies might not meaningfully affect student behavior. For example, schools that are "online" and schools that are "in-person" may both see large numbers of students returning to off-campus housing and exhibiting similar behavior. Some use this as justification for not investigating how variation in school reopening policy changes outcomes.

I have 2 observations. First, if it is in fact true that school reopening policies don't matter for local transmission, then that's a fairly strong result that undercuts rationale behind school's decisions. Second, I suspect that the extent to which school reopening policies change student behavior depends largely on the percentage of students living off campus. At schools with entrenched off campus housing presences, students were likely locked in to off-campus leases before the pandemic began, and thus student behavior would not be very sensitive to school policies. At schools without off campus housing presences, student behavior figures to be more sensitive to school policies, and thus school policies will have a stronger effect on local community COVID situations.



