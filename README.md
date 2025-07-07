# TITLE  
The Lingering Challenges of Aging Tunnel Infrastructure in Japan

## SHORT DESCRIPTION OF WHAT YOU AIMED TO ACCOMPLISH
- Clarify the current state and issues of aging infrastructure in Japan using data on tunnels across the country.

## SHORT DESCRIPTION OF YOUR FINDINGS
- Analysis of the data on unrepaired tunnels revealed inconsistencies, suggesting that the very definition and approach to aging countermeasures may be fundamentally flawed.

## SUMMARY OF THE DATA COLLECTION PROCESS, WITH LINKS / OVERVIEW OF THE DATA ANALYSIS PROCESS

1. **Number of tunnels by aging risk across Japan**  
   - Obtained PDF data showing the number of tunnels by prefecture and risk level, published by each supervising authority.  
   - Converted the data to CSV using Python and aggregated it with pandas.  
   - [MLIT Tunnel Data](https://www.mlit.go.jp/road/sisaku/yobohozen/yobohozen_maint_r05.html)

2. **Number of tunnels by prefecture**  
   - Further aggregated the data from step 1 using pandas.  
   - Added prefectural latitude and longitude information using the Geospatial Information Authority of Japan API for mapping.  
   - [GSI API](https://vldb.gsi.go.jp/sokuchi/surveycalc/api_help.html)

3. **Number of tunnels by risk level and repair status by prefecture**  
   - Scraped data from a website listing each tunnel's address, risk level, and repair status.  
   - Converted the collected data into prefecture-level summaries using pandas.  
   - Created several graphs and images, and finalized the visualizations to be made with Datawrapper by simplifying the data.  
   - [MLIT Tunnel Data](https://www.mlit.go.jp/road/sisaku/yobohozen/yobohozen_maint_r05.html)

4. **Actual photos**  
   - Verified tunnel information using Google Maps, actual maps, and local government websites by manual inspection.

## NEW SKILLS, APPROACHES, AND GROWTH DURING THE PROJECT

- Data scraping using a method where previous data disappears and new data appears with each scroll.
- Displaying map data using Datawrapper.

## THINGS YOU TRIED TO DO OR WANTED TO DO BUT DID NOT HAVE THE SKILLS/TIME

- Could not find an API for traffic volume. If I had more time, I wanted to calculate tunnel usage rates across Japan.
- Would like to improve my sense of design for images.
