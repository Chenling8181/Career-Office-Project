# Job Description Parser

The Job Description Parser is a tool designed to help you efficiently analyze job listings based on specific criteria. Whether you're a job seeker looking for relevant positions or a recruiter trying to find the perfect candidate, this parser can streamline your search process.

## Usage

### Input Parameters
- **Search Query**: The job title or keyword you're searching for.
- **Location**: The location where you want to find job listings.
- **Keywords in Description**: A list of keywords to search for in job descriptions, in order of preference.
- **Keywords in Title**: A list of keywords to search for in job titles. Matching these keywords increases the rating of the job.
- **Keywords to Exclude**: A list of keywords to exclude from job titles. Matching these keywords sets the rating of the job to zero.
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
