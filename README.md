# Job Description Parser

The Job Description Parser is a tool designed to help you efficiently analyze job listings based on specific criteria. Whether you're a job seeker looking for relevant positions or a recruiter trying to find the perfect candidate, this parser can streamline your search process.

## Usage

### Input Parameters
- **Search Query**: The job title or keyword you're searching for.
- **Location**: The location where you want to find job listings.
- **Ordered Keywords**: A list of keywords to search for in job descriptions, in order of preference.
- **Title Keywords**: A list of keywords to search for in job titles. Matching these keywords increases the rating of the job.
- **Exclude Keywords**: A list of keywords to exclude from job titles. Matching these keywords sets the rating of the job to zero.
- **Pages**: The number of pages of job listings to search on Indeed (up to 100).

### Output
The tool returns a DataFrame of job listings, sorted by a "rating" metric based on the ordered list of keywords. You can download the full DataFrame as an Excel sheet for further analysis.

## Example Workflow

1. **Generate Example Job Descriptions**: Create a couple of example job descriptions to work with.
2. **Get Real Job Description Data**: Obtain real job description data from the careers office.
3. **Learn/Research Keyword Extraction**: Learn how to extract keywords from text effectively.
4. **Extract Keywords**: Attempt to extract keywords from example job descriptions.

## Notes
- The tool is flexible and can be adapted to different use cases.
- The ordering of keywords in the "Keywords in Description" parameter affects the rating of job listings.
- Keywords in the "Keywords in Title" parameter take precedence over the ordered list of keywords.

By using the Job Description Parser, you can efficiently sift through job listings to find the most relevant opportunities or candidates.

# Student-Job Matcher

This algorithm, created in Python, is designed to help students from the different IEOR programs be matched to certain online jobs based on their skill sets and interests.

## Usage

Data should be collected on students from the different MSOR programs through a Google Form. For each student, they should be surveyed on their Interests, Target locations, and Summer Status or Internship (the column can be labeled either way, and this represents what they are looking for in the summer). There can be additional data collected in the Google Form, but these were the ones we targeted in this code program. From here, the survey data should be converted into Excel .csv files. There can be multiple .csv files, one for each program. Note that the ID is unique and anonymized for each individual and follows the format of MSPROGRAM_01, MSPROGRAM_02, etc. (comprising MSBA, MSFE, MSIE, MSMSE, or MSOR).

Download all of the .csv files into a folder, and find the folder path to it. In the first block of code, there is a variable called “folder_path”. For example:
```
folder_path = '/Users/gwendolynseto/Downloads/MS_IEOR_Data'
```
Replace the content of the folder path with your local folder path to the data. From here, the code should be able to run.

### Output

The algorithm will output, for each student, various jobs that they are matched to based on their interests and skills. This information can then be transferred over to the students so they can apply for internships. This will serve as a tool in the job-hunting process, as students will likely find something that is relevant and in the industry they are looking for.

## Notes

The way the algorithm works is that student data is extracted from the Excel sheets. A web scraping algorithm goes on a site (such as Indeed) and finds relevant job information. Based on the student’s major, career interests, and workplace locations of interest, the algorithm returns relevant job results.
