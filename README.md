minneapolis-raw-election-results-2013
=====================================

Raw Ranked Choice Voting (RCV) election results from the City of Minneapolis municipal general election on November 5, 2013.

## This is not ready for use yet!

I'm not done processing data. Don't use this.

## Limitations

This dataset does not maintain ballots as separate elements that include votes for multiple races, meaning ballots are individualized only on a per-race basis. As an example, it would be impossible to find a connection between voters choosing a particular mayoral candidate and who they voted for in other races on their ballot. For that reason, the ballots are not combined to a single table, as technically a 'ballot' would be duplicated in that form. This is a limit of the original dataset from the City.

## Folders

* source-xlsx: Raw .XLSX source files from the City of Minneapolis 
* source-tabulations-xlsx: Raw .XLSX tabulation files from the City of Minneapolis (useful for verification)
* source-tabulation-pdf: Human-readable .PDF tabulation results from the City of Minneapolis (useful for verification)
* unprocessed-csv: A direct conversion of the source-xlsx .XLSX files to .CSV
* processed-sql: Contains an .SQL file of all ballots for all races (see limitations above)
* processed-csv: Contains individual .CSV files of all ballots for all races

## Processed Schema

* ballot_id: Sequential ID for indexing purposes only. It is not known what order this data is in (processed).
* precinct_text: A string that represents the ward and precinct (e.g. MINNEAPOLIS W-13 P-06) indicates the ballot was made in Ward 13, Precinct 6.
* ward_number: The ward number the ballot was cast in (processed).
* precinct_number: The precinct number the ballot was cast at (processed).
* choice_1_text: A string that represents the name of the candidate chosen for the ballot's first choice.
* choice_1: 
* choice_2_text: A string that represents the name of the candidate chosen for the ballot's second choice.
* choice_2: 
* choice_3_text: A string that represents the name of the candidate chosen for the ballot's third choice.
* choice_3: 
* count:

## Disclaimer

Although best efforts were made to ensure data accuracy, this is not the official data source and unknown errors could have been introduced. This repository contains data that has been modified for use from its original source, vote.minneapolismn.gov, the official website for the City of Minneapolis Elections & Voter Services department. Nobody, including but not limited to the City of Minneapolis, makes claims as to the content, accuracy, timeliness, or completeness of any of the data provided herein.

THE SOFTWARE/DATA IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE/DATA.

