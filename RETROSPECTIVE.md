# Sprint retrospective: Netflix Executive Dashboard Sprint

## Sprint summary

### Sprint goal	
Deliver a working executive dashboard prototype built on the 500-record viewing and ratings dataset, with 5 KPIs, filters for membership, genre and country, validated calculations and a stakeholder review.

### Result	
Goal met. All 5 KPIs and 3 filters work, KPI calculations were checked against the raw data, and the prototype was reviewed.
### Cards completed	
12 of 12 sprint cards (3 backlog cards deferred as planned)
### Risks	
Both risks were managed and neither became a blocker
### What went well
#### The Kanban board made blockers visible early. 
The data-cleaning card (4) sat in "In progress" the longest, so the team saw the delay at the daily stand-up and not at the end.

#### Writing KPI definitions first (card 2) prevented arguments. 
Everyone calculated average rating the same way, from the individual ratings.

#### Wireframe review before building (card 6) saved rework. 
The Product Owner trimmed the front page to 5 KPIs before any code was written.

#### The 2-cards-per-person limit 
kept work moving and stopped cards piling up in "In progress".

#### Validation caught a real difference. 
The dataset's Average_Ratings column and the dashboard's filter-based averages needed to be explained, and the analyst caught this during card 5.

### What did not go well
#### Data cleaning took longer than estimated
which squeezed usability testing (card 9).
#### Stakeholder feedback came late. 
The review meeting was booked for the end of the sprint, which left little time to act on comments.
#### The data limited the KPIs. 
#### The dataset has views and ratings only
so financial KPIs such as revenue, churn and cost per viewing hour could not be shown.
#### The data is synthetic
so the insights show how the dashboard works but are not real findings about Netflix.
#### Board housekeeping slipped
Some cards stayed in the wrong column for a day or two, so the board was occasionally out of date.

### What we learned
Data tasks are the biggest source of uncertainty, so estimate them with a buffer.
Fewer KPIs presented clearly are better than many presented densely.
A KPI needs one written definition before anyone builds it.
The "Done only after review" rule worked, but it needs a named reviewer on each card.

#### Action items for the next sprint
#### Action	                                                                                            
Add a 20% buffer to data-engineering estimates	 - Owner: Scrum Master 
#### Action 
Book the stakeholder review in the first week, not the last day	   - Owner: Product Owner
#### Action
Add revenue, churn and streaming-quality data so financial KPIs can be included	 - Owner: Data Engineer
#### Action
Build the backlog items: genre drill-down, mobile view and automated daily refresh  - Owner: Dashboard Developer
#### Action
Name a reviewer on every card before it moves to "In review"	- Owner: Scrum Master
Update the board at the end of each stand-up	 -Owner - Everyone

### Sprint rating
Team confidence in the next sprint: 4 out of 5. The process worked, and the main risk is still data availability.
