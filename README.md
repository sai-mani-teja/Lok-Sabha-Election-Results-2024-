# Lok-Sabha-Election-Results-2024-
Election Results Analysis Report


Data Collection:

The election results data was collected by scraping multiple websites using Python libraries like requests and BeautifulSoup. Each website URL contained a unique identifier corresponding to a specific political party's election results. These identifiers were stored in a list (l) and represented parties in descending order based on the seats they won.

Data Scraping Methodology:
Using a loop, each URL was accessed, and the HTML content was parsed to extract relevant election results:

URL Structure: Each URL was structured as https://results.eci.gov.in/PcResultGenJune2024/partywisewinresultState-{i}.htm, where {i} represented the unique identifier for a party.

Data Extracted: For each webpage, data such as Parliament Constituency, Winning Candidate, Total Votes, Margin, and Party were extracted from HTML tables using BeautifulSoup.


Data Analysis and Key Insights:

Based on the collected data, the following key insights were generated:

1) Parliament Constituency with the highest total votes:
Identified the constituency where the highest number of votes were cast.

2) Parliament Constituency with the lowest margin of victory:
Highlighted the constituency with the smallest margin between the winning and runner-up candidates.

3) Parliament Constituency with the largest margin of victory:
Showcased the constituency with the widest gap between the winning and runner-up candidates.

4) Party with the highest total votes:
Determined the party that received the highest cumulative votes across all constituencies.

5) Top 5 winning candidates by total votes:
Listed the candidates who received the most votes in their respective constituencies.

6) Top 5 constituencies with highest voter turnout:
Identified the constituencies with the highest voter participation based on total votes cast.

7) Average margin of victory by party:
Calculated the average margin of victory for each party, indicating their strength in winning constituencies.

8) Number of close contests (margin < 5000 votes):
Counted the number of constituencies where the winning margin was less than 5000 votes, indicating closely contested races.

9)Average total votes by party:
Analyzed the average number of votes received by each party across all constituencies they contested.

10) Winning candidates with the least total votes:
Highlighted candidates who won with the fewest votes, reflecting less popular support in their constituencies.

Value of the 'Party' Attribute:

The introduction of the 'Party' attribute, derived from the serial number (S.No) assigned to each party, proved crucial in:
Analysis Facilitation: Enabling aggregation and comparison of results across different parties.
Insight Generation: Providing context to key insights such as average votes by party and identifying parties with significant electoral margins.

Conclusion:
The combination of web scraping to collect election data and subsequent analysis using pandas facilitated the extraction of meaningful insights from the election results. The process demonstrated the utility of Python programming in data-driven tasks, showcasing how structured data collection and analysis can inform decision-making in electoral analysis.
