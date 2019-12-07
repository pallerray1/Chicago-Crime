# Chicago Crime

<img src="./assets/CTA_L_at_speed_looking_south_on_lasalle.png"/>

##  Problem statement

To distill information that would be of utility and benefit to those individuals and organizations that have as their intent the desire and willingness to improve life in the City of Chicago.

## Executive Summary

To gather and use data to make informed decisions, guide behavior, and improve outcomes  --  whether for an individual or an institution -- is the raison d'etre for data science.  The historical images of Al Capone to the current rendering of "Chi-raq" makes for a highly charged atmosphere, with openings to inflame emotions or distort realities.  The use of reason, science, and an exploratory spirit to dive into volumes of raw crime data to hopefully (but without guarantees) extract meaningful insights was the motivating driver.

The largest overarching theme that was discovered, and gives rise to good confidence that the results could be employed to individuals' and the City's benefit,  was the cyclic nature of criminal acts.  When combined with knowledge of (a) different types of crimes having different likelihoods at various hours of the day and (b) each local district's distributions of offense types,  creative ideas both grandiose and more modest can be implemented.

In one sentence, the overall crime rate has shifted slightly down during the seven year interval studied November 2012 to November 2019, with the majority in the first two years and a more steady state since.

Overall cycles or trends identified, together with each one's 'period':

  1) Yearly cycle: troughs in February, peaks in August, returning to trough in February
  2) Daily cycle:  troughs at 5 to 6 AM, peaks at roughly 6 to 7 PM, a noticeable spike from cycle at around Noon
  3) Daily cycle by type:  Violent crimes of homicide, battery, and robbery follow the overall daily crime cycle but have a phase shift
        that places their peaks and valleys around 2 to 3 hours after those of the overall crimes daily cycle.
  4) The combined day grouping of Friday/Saturday/Sunday has a crime rate cycle of, over the course of a year, 4 peaks and 4 troughs. It does not punch at it's own weight --- it is either additive or subtractive depending on where it is in its own cycle.
  5) The violent crimes of homicide, battery, and robbery have greater representation in the Friday/Saturday/Sunday groupings.
  6) Deceptive practices mostly takes place at two rocket-launch spikes, namely, around 8 AM and then 12 Noon.
  7) A very weak (but identifiable) trend of the first and third weeks of the month being heavier than of the second and fourth weeks.

  At the police district level, information can be gleaned that could be useful to each individual district. Streets and crime types, for instance.  Too many permutations to be mentioned here.

  And finally, hypothesis testing was employed to validate 2 common heuristics.  Indeed, "when it gets hot, people get shot" tests TRUE! But when "the full moon comes out, so do the crazies" proved itself bunk.


## Recommendations

There are many potential end users.
  Citizens and tourists can utilize their alertness more effectively depending on when and where they will be.
  Police Department shift schedulers could be assisted.
  Officer deployment (subject to any instituted constraints)

Of deployments grandiose and more modest:
  Instead of an immediate grand proposal that would be difficult to implement (money, manpower, and inertia), a modest proposal to get initiative rolling and be useful could be as follows:  no large scale equipment purchases needed, use the existing radio;  have an auto-generated one or two sentence statement generated for each shift for each district that auto-calculates a net plus or minus crime day based upon all the cycles present on any given day, supplement streets or blocks or crime types that are relevant to a given district; and robo-speech generate the broadcast to each officer's radio

  The officers may get annoyed by a short but everyday update synopsis put out by the research department back at headquarters;  so employ some worldly wisdom to deliver it.  

  Take the worldly mungerism that says:  If you start with raisons and then add rabbit turds, what you wind up with is turds.  
  Adopt and contortion it.  Start with raisons and add turds, but at least sugar coat the turds.  Do that by broadcasting at the officer's break time a nice reminder that he/she has a break time coming, and then say the synopsis. Maybe something along this order:

    "Good morning.  
    A reminder that you've reached your break time.
    The odds today suggest that it's a PLUS crime day.
    The east-west street on your beat that could be of interest is Madison.
    The north-south street that could be of interest is Pulaski.
    The eggheads back in research wish you a safe shift."




  ## Notebooks

  ---
  ** Code **
  * [Analysis: Day of Week including Friday/Saturday/Sunday Groupings](code/analysis_1_day_of_week_especially_fri_sat_sun.ipynb)
  * [Analysis: Hours of the Day](code/analysis_2_hours_of_the_day.ipynb)
  * [Analysis: Days of the Month,  Weeks of the Month](code/analysis_3_days_of_the_month_weeks_of_the_month.ipynb)
  * [Analysis: Daily, Monthly, & Friday/Saturday/Sunday Monthly](code/analysis_4_daily_monthly_fri_sat_sun_crime_rates.ipynb)
  * [Analysis: For the Districts](code/analysis_5_for_the_districts.ipynb)
  * [Full Moon Hypothesis](code/full_moon_hypothesis_test.ipynb)
  * [High Summer Temperature Hypothesis](code/high_summer_temperature_hypothesis_test.ipynb)
  * [Preliminary Read In/Prep Data](code/prelim_read_prep_data.ipynb)

---
** Data **

[City of Chicago Data Portal: Crimes 2001 to Present](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2)

---
** Presentation **

[Slide Deck: Chicago Crime 2019 - Intent to Inform](Chicago_Crime.pdf)
